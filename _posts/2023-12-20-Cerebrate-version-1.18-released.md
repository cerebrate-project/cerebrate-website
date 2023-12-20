---
title: Cerebrate version 1.18 released including new features, improvements and bugs fixed 
tags: release 
---

## v1.18 (2023-12-20)

![Cerebrate bulk org import from MISP](https://github-production-user-asset-6210df.s3.amazonaws.com/3309/291860287-01ba669c-6bfb-4081-ba3a-c3da724de705.png)

### New

* [settings:inbox.data_change_notify_for_all] Added setting to be more verbose for data changes. [Sami Mokaddem]

* [CRUD:Filtering] Added support of options in index filtering modal. [Sami Mokaddem]

### Changes

* [version] bump. [iglocska]

* [inboxes:filtering] Populate username with eligible users in filtering modal. [Sami Mokaddem]

* [crud:index] Include all meta-fields regardless of user's preference when in REST context. [Sami Mokaddem]

* [MISP connector] added bulk org pull. [iglocska]

### Fix

* [inboxes:index] Fixed pagination target key. [Sami Mokaddem]

* [component:CRUD] Make sure not to override table aliases when paginating. [Sami Mokaddem]

* [individual:validation] Enforce email format to be a valid email address. [Sami Mokaddem]

* [behavior:notifyAdmins] Fixed typo in date serialization. [Sami Mokaddem]

### Other

* Merge branch 'develop' [iglocska]

* Merge branch 'develop' of github.com:cerebrate-project/cerebrate into develop. [Sami Mokaddem]

Thanks to all the contributors and users who reported bugs and feature ideas! 

