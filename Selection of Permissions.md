# Decision record template by Michael Nygard

This is the template in [Documenting architecture decisions - Michael Nygard](http://thinkrelevance.com/blog/2011/11/15/documenting-architecture-decisions).
You can use [adr-tools](https://github.com/npryce/adr-tools) for managing the ADR files.

In each ADR file, write these sections:
# Assignment: Architectural Decisions
# 2023-10-10
# Yuta Kikuchi
# Scenario 1
# Selection of permissions it needs

## Status

Proposed.

## Context

Since the application needs to have accesses to hardware functions of the user's device in order to have all of the functions work together effectively, it needs to be specified what kinds of permission the application needs.

## Decision

Necessary permissions are listed below:

- Access to device storage: required to store and synchronize data in offline mode.
- Access to network status: required to switch between offline and online modes.
- Receive push notifications: required to receive notifications and keep users informed.
- Access to the camera: required for image upload.
- Access to location information: required to provide localized information.

## Consequences

With these changes, the app will be able to meet the requirements and provide all of its functions to users such as the use of the app in an offline environment, the utilization of push notifications, and displaying of product images.
