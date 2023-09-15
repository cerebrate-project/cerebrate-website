---
title: Cerebrate version 1.15 released including new features, improvements and security fix (CVE-2023-41363)  
tags: release 
---

## Cerebrate version 1.15 released including new features, improvements and security fix (CVE-2023-41363) 

### Changes

* [version] bump. [iglocska]

* [misisng] change. [iglocska]

* [internal] fetch first role if no default is set. [iglocska]

* [command:summary] Consider perm meta-fields addition/deletion as uesr edit. [Sami Mokaddem]

* [config] Force usage of secure cookie for session and csrf protection. [Sami Mokaddem]

* [component:CRUD] Include meta-fields in REST queries and clever pagination support for REST queries. [Sami Mokaddem]

* [command:summary] Added support of user MetaFields. [Sami Mokaddem]

  Allow to show addition and deletion of user metafields such as the ones used for permissions

### Fix

* [security] user settings editable by arbitrary user fixed. [iglocska]

  - as reported by Infigo on behalf of ENISA - [CVE-2023-41363](https://cvepremium.circl.lu/cve/CVE-2023-41363)

* [internal] user add fix attempt #2. [iglocska]

* [userSettings:edit] Correctly pre-select user to be edited. [Sami Mokaddem]

### Other

* Merge branch 'develop' [iglocska]

* Merge branch 'main' into develop. [iglocska]

* Update INSTALL.md. [Andras Iklody]

* Update INSTALL.md. [Andras Iklody]

  some minor fixes


