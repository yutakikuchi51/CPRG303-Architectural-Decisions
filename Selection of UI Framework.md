# Decision record template by Michael Nygard

This is the template in [Documenting architecture decisions - Michael Nygard](http://thinkrelevance.com/blog/2011/11/15/documenting-architecture-decisions).
You can use [adr-tools](https://github.com/npryce/adr-tools) for managing the ADR files.

In each ADR file, write these sections:

# Assignment: Architectural Decisions
# 2023-10-10
# Yuta Kikuchi
# Scenario 1
# Selection of UI Framework

## Status

Proposed.

## Context

In the requirements given by the company, there are issues that we need to resolve, and they affect the selection of the UI framework.
Since the client requires the application to support offline mode which still allows users to browse products and view their order history, we are in need of coming up with an idea about how the app's behavior is going to be, and deciding on suitable UI framework to implement these functions into the app.

## Decision

The selection decided to use React Native for the project.
One of the reasons is React Native enables developers to implement some fundamental functions so that users can have a high-quality UX while the app is offline. More specifically, we can implement functions such as usage restriction which restricts some functions and is notified that it is currently offline, caching which enables temporary saving of data in local storage, and request queue which executes all requests made while being offline after the internet connection is back.

## Consequences

It can be assumed that the decision will be effective to build an application that meets the client's requirement, and there will be an additional advantage of the ease of development when it comes to building an app for multiple platforms.
