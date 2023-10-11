# Decision record template by Michael Nygard

This is the template in [Documenting architecture decisions - Michael Nygard](http://thinkrelevance.com/blog/2011/11/15/documenting-architecture-decisions).
You can use [adr-tools](https://github.com/npryce/adr-tools) for managing the ADR files.

In each ADR file, write these sections:
# Assignment: Architectural Decisions
# 2023-10-10
# Yuta Kikuchi
# Scenario 1
# Selection of the type of application(Native, Web, or Hybrid Application)

## Status

Proposed.

## Context

There are several issues that motivated me to make this decision in terms of selecting the type of application to build for this project.
One of the issues is that the retail company wants the app to support offline mode while users can utilize some functions such as viewing order history and browsing products.
There is also a requirement that the company wants us to consider, which is that they want to send push notifications because of the need to notify customers about order updates, brand-new product arrivals, and exclusive offers.

## Decision

To address those issues, we decided to develop Native Application for this project. 
First of all, it is considered that building a native application is the most appropriate option chosen for this case because a native application can work offline on the user's device, whereas web and hybrid applications have difficulty being built to be able to support offline mode despite the fact that it is still possible to do it if we additionally consider other factors such as offline data storage.

Secondly, there is another reason to reach the decision. When it comes to considering the use of push notifications that the company requires, a Native app is still a reasonable option to select because a Native app can directly have access to the operating system which allows an application to integrate with the push notification functionality. It means that the system will be able to work with the push notification more seamlessly.

## Consequences

As an expectation, we assume that it will be a longer development time and more costly if there is a need to develop the application for multiple platforms like a native Android application or a native iOS application. It probably has an effect when it comes to efforts for maintenance and testing.
