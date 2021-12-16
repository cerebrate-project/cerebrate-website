---
title: Cerebrate version 1.2 released - the open source companion to ISACs, CSIRTs and SOCs 
tags: release 
---

### Cerebrate 1.2 released - the open source companion to ISACs, CSIRTs and SOCs

In the scope of the [Open platform and tools to facilitate the collaboration among Computer Security Incident Response Teams](https://www.enisa.europa.eu/news/enisa-news/open-platform-and-tools-to-facilitate-the-collaboration-among-computer-security-incident-response-teams) project funded by the EU commission, [CIRCL](https://www.circl.lu/) is pleased to announce the 1.2 release of Cerebrate, an open source security orchestration tool for CSIRTs and SOCs.

Cerebrate v1.2 released with a host of bugs resolved and some slight modifications to the handling of the user objects.

### User objects are now tied to organisations

Prior to this versions, the only way to bind a user to an organisation was via the related individual object. This caused issues with users belonging to multiple or no organisations in practice, both of which are valid for individuals, but make access control difficult.

With the current release, users are now tied to organisations and the access control is restricted accordingly. If the intent is to allow a user to act on behalf of multiple organisations, simply add multiple users to an existing individual, one for each organisation, to achieve the expected result.

### Improved ACL handling and multiple fixes

- [ACL Helper] check access for controller / action pair for given user
- Many forms improved

For more details of changes in the [Cerebrate changelog](https://www.cerebrate-project.org/Changelog.txt).

For more information, you can visit the [cerebrate project](https://www.cerebrate-project.org) website. You can also follow the [MISP](https://twitter.com/MISPProject) and [Cerebrate Twitter account](https://twitter.com/cerebrateproje1). Contact [CIRCL](https://www.circl.lu/contact/) for partnerships, ideas and feedback.

