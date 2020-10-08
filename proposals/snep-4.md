---
SNEP: 4
title: Support alternate storage systems in Daemon
author: Cassio Pennachin <cassio@singularitynet.io>
discussions-to: [Daemon](https://github.com/singnet/snet-daemon)
status: Draft
type: Standard
category : Components
created: 2020-10-08
requires (*optional): 
replaces (*optional): 
---

##
**Simple Summary**

Enable the daemon to use different storage system apart from etcd

##
**Abstract**

Enhance the daemon so that it can work with any type of storage such as RDBMS, MongoDB etc 

##
**Motivation**

The [SingularityNET daemon](https://github.com/singnet/snet-daemon) is the adapter that a service can use to interface with the SingularityNET platform.

The daemon is a [sidecar proxy](https://docs.microsoft.com/en-us/azure/architecture/patterns/sidecar), —a process deployed next to a core application (the AI service, in this case) to abstract away some architectural concerns such as logging and configuration as well as entire platform aspects, such as the interaction with smart contracts or even the decision to use the Ethereum Blockchain.

Currently the daemon uses etcd as its storage to maintain state. We would like to enable the daemon to work with any other storage system such as 

*   Relational Databases
*   NoSQL stores such as MongoDB, Cockroach DB

This will enable service developers to leverage any existing services or opt for managed services. They would not be forced to set up an etcd cluster to run the daemon.

##
**Technical Specification**

*   Daemon uses etcd as storage to store context related to
    *   [Payments](https://dev.singularitynet.io/docs/platform-dev/daemon-channel-storage/)
    *   Free Call Usage at an organization level.
*   Enable the use of any other storage system instead of etcd
*   Service developer should be able to choose the storage system to use while starting up the daemon
*   Daemon must initialize the chosen storage system and work seamlessly with clients and AI services as before.
*   Daemon must be able to maintain state as it did before across groups
*   Daemon should be able to service requests and manage payments as before
*   Daemon should be able to handle issues with the storage system gracefully


##
**Test Cases & Community Discussions**

All existing unit test suites in [https://github.com/singnet/snet-daemon](https://github.com/singnet/snet-daemon) must pass.


## 
**Copyright**

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
