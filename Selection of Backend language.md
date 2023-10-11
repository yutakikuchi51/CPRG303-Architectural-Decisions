# Decision record template by Michael Nygard

This is the template in [Documenting architecture decisions - Michael Nygard](http://thinkrelevance.com/blog/2011/11/15/documenting-architecture-decisions).
You can use [adr-tools](https://github.com/npryce/adr-tools) for managing the ADR files.

In each ADR file, write these sections:

# Assignment: Architectural Decisions
# 2023-10-10
# Yuta Kikuchi
# Scenario 1
# Selection of Backend Language

## Status

Proposed.

## Context

Since we will build an application that handles user's personal information and payment information, the system should be secure. Also, the retail company currently plans to expand its customer base internationally in the long term, so it is desirable to have the application scalable and easy to maintain.
Additionally, we are in need of thinking about how to build the app that can be used by a larger number of users as the company expands its customer base internationally.

## Decision

The selection was made to use Java as the backend language.
Java is widely used as a backend language because of being an incredibly secure language, so it can contribute to building a robust application that handles various information of users.
In addition, Java is extensively used in industries related to mobile applications, especially Android applications. Considering that the company currently has an idea of expanding its business internationally and Android holds a huge market share around the world, it is reasonable to select Java as a backend language to build a popular application.

## Consequences

The selection will bring about desirable effects for meeting the requirements such as the ease of maintenance in a long term, and the improvement of the app's security. 
