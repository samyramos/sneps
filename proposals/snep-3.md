---
SNEP: 3
title: Swift SDK
author: Cassio Pennachin <cassio@singularitynet.io>
discussions-to: [Class Diagram](https://github.com/singnet/snet-sdk-java#class-diagram)
status: Draft
type: Standard
category : Components
created: 2020-10-08
requires (*optional): 
replaces (*optional): 
---

##
**Simple Summary**

Built an SDK in Swift

##
**Abstract**

SDK is a tool for AI customers to make calls to services. It simplifies the process of integrating with SingularityNET services and provides all the plumbing to interact with the Daemon.

All SDKs come with an out of the box Payment Strategy so can be used as is. AI Consumers can provide their own payment strategy based on the way they plan their transactions. This flexibility enables consumers to use the SDK in a myriad ways.

A richer set of SDKs will further enhance usage of the platform. With a Swift SDK we can enable the creation of iOS apps that can leverage different AI Services that we have

##
**Motivation**

We currently have SDKs in 

*   Python ([https://github.com/singnet/snet-cli/tree/master/packages/sdk](https://github.com/singnet/snet-cli/tree/master/packages/sdk))
*   NodeJS ([https://github.com/singnet/snet-sdk-js](https://github.com/singnet/snet-sdk-js))
*   Java ([https://github.com/singnet/snet-sdk-java](https://github.com/singnet/snet-sdk-java))

##
**Technical Specification**

*   Build an SDK in swift capable of being used in all iOS devices 
*   SDK should expose the same interfaces as exposed by the Java SDK 
    *   Class Diagram - [https://github.com/singnet/snet-sdk-java#class-diagram](https://github.com/singnet/snet-sdk-java#class-diagram)
    *   SDK Class definition - [https://github.com/singnet/snet-sdk-java/blob/master/sdk/src/main/java/io/singularitynet/sdk/client/Sdk.java](https://github.com/singnet/snet-sdk-java/blob/master/sdk/src/main/java/io/singularitynet/sdk/client/Sdk.java)
    *   Service Class - [https://github.com/singnet/snet-sdk-java/blob/master/sdk/src/main/java/io/singularitynet/sdk/client/ServiceClient.java](https://github.com/singnet/snet-sdk-java/blob/master/sdk/src/main/java/io/singularitynet/sdk/client/ServiceClient.java)
    *   Default Payment Strategy - [https://github.com/singnet/snet-sdk-java/blob/master/sdk/src/main/java/io/singularitynet/sdk/client/PaymentStrategy.java](https://github.com/singnet/snet-sdk-java/blob/master/sdk/src/main/java/io/singularitynet/sdk/client/PaymentStrategy.java)

##
**Test Cases & Community Discussions**

Unit test on the same lines as provided in the [Java SDK](https://github.com/singnet/snet-sdk-java/tree/master/sdk/src/test) should be given and should pass


## 
**Copyright**

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
