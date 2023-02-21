---
title: Cerebrate 1.12, including new features, improvements and bug fixes. 
tags: release 
---

We are pleased to announce the immediate availability of Cerebrate 1.12, including new features, improvements and bug fixes.

## New features

- Get the audit logs associated to any entities generating log entries when in the `{controller}/view` scope
- New meta-templates and meta-fields migration strategies:
    - `update_existing`, `delete_all`, `update_existing`
    - `update_existing` has been set as the default strategy; replacing `create_new`
- New setting added, allowing the disabling of user deletions
- New UI components to streamline user interactions
- New `fastEnrolment` CLI tool  to quickly enroll users, organisations and individual

## Improvements

- Improved UI of the `Notification/DataChange` Inbox processor
- Meta-fields synchronisation by using `meta_template_directory_id`
- UI description and documentation for update strategies and conflict resolutions
- Refactoring of the generic Bootstrap UI elements. Adding support for more options and including extensive component documentation
- Previewing remote Cerebrate instances now support pagination, filters and synchronisation status

## Fixes

Several annoying issues have been resolved, especially in regards to meta-template updates and meta-fields migration.
For a full list of changes, refer to the [changelog](https://www.cerebrate-project.org/Changelog.txt)

## Shout outs

Thanks to all contributors as well as all users that have let us know about issues, improvement ideas and generally sanity checking what we do. 

A huge [thank to the EC](https://www.enisa.europa.eu/news/enisa-news/open-platform-and-tools-to-facilitate-the-collaboration-among-computer-security-incident-response-teams) for the co-funding for the development of Cerebrate under "Connecting Europe Facility – Cybersecurity Digital Service Infrastructure Maintenance and Evolution of Core Service Platform Cooperation Mechanism for CSIRTs – MeliCERTes Facility” (SMART 2018/1024) contract.

## Screenshots of new features
### New migration strategies
![image1](https://user-images.githubusercontent.com/6977223/220361262-e05e9e30-800b-4d42-88a6-9bc069f5bad2.png)
![image2](https://user-images.githubusercontent.com/6977223/220361340-70bd3a97-cf66-41fd-9981-41ab78e7b8c4.png)
![image3](https://user-images.githubusercontent.com/6977223/220361446-886b7031-c41c-4b0b-8b34-c4e351d1f8df.png)
### Audit logs on every entity
![image4](https://user-images.githubusercontent.com/6977223/220361494-d902d84f-6346-4559-b3df-29852d324875.png)


