# Decision record template by Michael Nygard

This is the template in [Documenting architecture decisions - Michael Nygard](http://thinkrelevance.com/blog/2011/11/15/documenting-architecture-decisions).
You can use [adr-tools](https://github.com/npryce/adr-tools) for managing the ADR files.

In each ADR file, write these sections:
# Assignment: Architectural Decisions
# 2023-10-10
# Yuta Kikuchi
# Scenario 1
# Selection of Data Storage

## Status

Proposed.

## Context

It is needed to consider how we utilize data storages to properly save and maintain data for the application, also the solution should be unique and suitable for this application because it will support offline mode.

## Decision

As a suggestion, utilizing multiple data storages types can be a way to safely handle and efficiently transmit data with a variety of functions the application has.
Specifically, we can use a local storage in user's side so that it enables users to browse products, view their order history, and access to any information related to the loyalty program feature while the app is offline. Also database on server side is the other storage type we can use to maintain information about products, user accounts, and orders.

## Consequences

The selection will make it possible that the application still work in an offline environment and users can still have an access to some of functionalities which don't require internet connection because of data stored on local storages.
