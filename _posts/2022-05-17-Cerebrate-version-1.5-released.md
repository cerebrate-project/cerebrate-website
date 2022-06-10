---
title: Cerebrate 1.5 released with a collection of improvements
tags: release 
---

# Cerebrate 1.5 released with a collection of improvements

We are happy to announce the 1.5 release of Cerebrate, a security, feature and usability release focusing on the various CSIRT use-cases and a user management revamp.

## Meta template rework

As of the 1.5 release, meta templates have received a host of new functionalities, including advanced search functionalities and special meta fields. The main objective was to enable organisations to capture constituency information for organisation, including CIDR blocks and AS numbers whilst also enabling users to find the correct PoC when searching for responsible parties by for example IP address.

## User management and keycloak rework

The strategy used to enroll and update users in keycloak has been reworked. Cerebrate is now the authoritative identity provider in our current vision, pushing changes to keycloak. We have also added recurring synchronisation mechanisms to the exchange. 

## Security

We have had a large penetration test conducted by Zigrin Security as a follow up of the rework of key aspects of Cerebrate such as user management. We have fixed a series of identified vulnerabilities and weaknesses along with identified usability bugs as part of this release. Besides just fixes, this also resulted in some additional security features such as a registration flood protection. For a full run-down of all fixes refer to the [changelog](https://www.cerebrate-project.org/Changelog.txt) and the [security page](https://www.cerebrate-project.org/security.html) for identified CVEs.

A massive thank you to the Luxembourgish army for funding the penetration test and thereby helping us ensure that our open-source toolchains remain secure and reliable.

## Various usability and UX improvements

A number of views have received overhauls and usability reworks - this is a continuous effort and we are looking for any feedback on how we can further ensure that Cerebrate doesn't get in your way of achieving your community management objectives. 

## Shout outs

Thanks to all contributors as well as all users that have let us know about issues, improvement ideas and generally sanity checking what we do. For a full list of changes, refer to the [changelog](https://www.cerebrate-project.org/Changelog.txt)

