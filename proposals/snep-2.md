---
SNEP: 2
title: Embedded Daemon
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

Run the daemon on embedded hardware

##
**Abstract**

Enhance the daemon so it can run on embedded hardware. This feature will enable various Internet of Things (IoT) use cases.

##
**Motivation**

The [SingularityNET daemon](https://github.com/singnet/snet-daemon) is the adapter that a service can use to interface with the SingularityNET platform.

The daemon is a [sidecar proxy](https://docs.microsoft.com/en-us/azure/architecture/patterns/sidecar), —a process deployed next to a core application (the AI service, in this case) to abstract away some architectural concerns such as logging and configuration as well as entire platform aspects, such as the interaction with smart contracts or even the decision to use the Ethereum Blockchain.

In its current form the daemon requires a server to run on dues to its CPU and memory requirements. In order to enable IoT use cases we need to have the daemon run on low-powered devices like the Raspberry Pi and other such devices. 

This will enable a whole range of usecases such as

*   Smart cities - Able to do basic video and audio process on the edge to enable street-scene analytics
*   Robotics - Able to be embedded in specialized robots

##
**Technical Specification**

*   Enable the snet daemon to be run on a Raspberry Pi 4 ([https://www.raspberrypi.org/products/raspberry-pi-4-model-b/specifications/](https://www.raspberrypi.org/products/raspberry-pi-4-model-b/specifications/)) or equivalent
*   Must be able to install and run the daemon on the Raspberry Pi device
*   Daemon must be able to run seamlessly for as long as the device is powered on.
*   Daemon must be able to maintain state 
*   Daemon must be able to proxy requests to the AI service (deployed on the same Raspberry Pi 4) while ensuring that payments are handled correctly.


 Test Cases & Community Discussions

All existing unit test suites in [https://github.com/singnet/snet-daemon](https://github.com/singnet/snet-daemon) must pass.

##
 **Copyright**

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
