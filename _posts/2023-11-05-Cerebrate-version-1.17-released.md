---
title: Cerebrate version 1.17 with new community management and orchestration features 
tags: release 
---

## Cerebrate v1.17 released with new community management and orchestration features

### Cerebrate topology view

With the release of 1.17, we have added a new interface to view and interact with your Cerebrate and its connected local tools as well as syncing broods.

By bringing up the topology view, Cerebrate will draw a layout of your setup using mermaid.js, showing identified issues and giving you easy access to managing the individual tools. 

![image](https://github.com/cerebrate-project/cerebrate/assets/3668672/8e92f62e-d33c-4c79-bf2c-01473c3611f0)

Using the local tools diagnostic interface, you can tie your own tool into this diagram, giving you an easy overview over misconfigured or misbehaving tools. Simply pivot to any of the sync connections or local tools to modify settings, execute updates and more.

### MISP connector updates

In tandem with the topology changes, the MISP connector has gone through a rework, allowing for more thorough diagnostics as well as easier exchange of contact items. 

The diagnostics will now warn about worker issues, outdated versions, or misconfigured MySQL / PHP setups. Wherever possible, quick remediation will also be offered via specific actions (such as "update MISP" or "restart workers").

![image](https://github.com/cerebrate-project/cerebrate/assets/3668672/0f87fe57-1b82-4107-b0cd-8a3e77a67154)

In order to make the exchange of organisations and sharing groups easier, the index interface has been reworked:

![image](https://github.com/cerebrate-project/cerebrate/assets/3668672/ebee80a0-dca4-41b3-98a9-a90f4bdbe130)

The new UI allows for comparing the data in Cerebrate to that in the connected MISP instance and pulling in a new / updated objects in a convenient multi-select function. In order to push organisation or sharing group data, you can use filter rules to define what will get pushed:

![image](https://github.com/cerebrate-project/cerebrate/assets/3668672/92762c89-4fe6-4c66-89cb-6f0ba090febd)

### Multiple fixes and improvements based on feedback from the CSIRT Network and ENISA

Thanks to our close collaboration, we have received a long list of ideas improvements and fixes in the past few weeks, resulting in a long list of fixes. These include highly improved filtering options for the user index, allowing sub-filtering based on metafields, a new CSV output format.

![image](https://github.com/cerebrate-project/cerebrate/assets/3668672/df6094dc-8195-4401-8abe-394d67f8e60d)

This becomes increasingly interesting when using Cerebrate with an IAM platform such as keycloak, where we manage subscriptions to certain services via metafields in Cerebrate. Being able to quickly view and interact with users that are subscribed to certain services is now a breeze.

### Various other fixes

A long list of fixes targeting our CI test suite as well as realigning the installed dependencies to newer versions (and resolving the issues they caused) were also included, for a full list of changes don't hesitate to check out our [Changelog](https://www.cerebrate-project.org/Changelog.txt).

