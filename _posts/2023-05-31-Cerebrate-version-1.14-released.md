---
title: Cerebrate version 1.14 released including new features, improvements and security fixes 
tags: release 
---

We are pleased to announce the immediate availability of Cerebrate 1.14, including new features, improvements and security fixes.

There is a new feature called enumeration collection to allow building dynamic list in Cerebrate.

We strongly recommend Cerebrate users to update to this latest version.

## v1.14 (2023-05-31)

### New

* [enumerations] added enumerations system. [iglocska]

  - for string entry fields, simply add lists of values to convert the text entry for values
  - helps with maintaining accurate lists
  - currently the fields that are valid targets are organisations.nationality, organisations.sector, organisations.type

* [enumerations] schema update added. [iglocska]

### Changes

* [version] bump. [iglocska]

* [CRUD] allow for sorting on related model fields. [iglocska]

  - some hacks to resolve issues with sorting on related fields

* [command:importer] Make sure to use the latest known version of the template. [Sami Mokaddem]

* [command:importer] Make sure to use the latest known version of the template. [Sami Mokaddem]

* [UI:saas] Clean-up css files and improved sidebar behavior and rendering for all themes. [Sami Mokaddem]

### Fix

* [users] added the country information to the index / view. [iglocska]

* [genericElements:formInfo] Removed unused portion of code. [Sami Mokaddem]

* [security] blind SQL injection in searchAll. [Sami Mokaddem]

  - As reported by Zigrin Security

* [meta-template-name-directory] Do not access property from null object. [Sami Mokaddem]

* [meta-template-direcotry:index] Pass baseurl to the anonymous function. [Sami Mokaddem]

* [metaTemplateDirectory:index] No static call anymore. [Sami Mokaddem]

* [template:registration] Correct usage of modal parameters. [Sami Mokaddem]

* [template:update_all] Correct usage of modal parameters. [Sami Mokaddem]

* [helper:formFieldMassage] Correctly check for key to avoid debug output. [Sami Mokaddem]

* [app:js] Removed log forgotten console log output. [Sami Mokaddem]

### Other

* Merge branch 'develop' [iglocska]

* Merge branch 'main' into develop. [iglocska]

* Merge branch 'main' into develop. [Sami Mokaddem]

* Merge branch 'develop' into main. [Sami Mokaddem]


## Shout outs

Thanks to all contributors as well as all users that have let us know about issues, improvement ideas and generally sanity checking what we do. 

A special thanks to NATO users for their feedback.
