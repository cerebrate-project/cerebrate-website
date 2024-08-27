---
title: Cerebrate v1.22 and v1.23 released with various bugs fixed and improvements
tags: release 
---

## Cerebrate - v1.23 (2024-08-27)

### New

* [metafield editor permission] added. [iglocska]

  - users/org admins/group admins/community admins can now only modify metafield data on any object if the permission is set for their role
  - Since some communities use this for ACL to secondary tools, this will allow them to restrict who can modify them

### Changes

* [version] bump. [iglocska]


## Cerebrate - v1.22 (2024-08-24)

### New

* [administration] allow group/org admins to edit individuals aligned to their managed orgs. [iglocska]

  - based on alignment

* [permissions] split of admin and community admin. [iglocska]

### Changes

* [migration] minor fix for rerunability. [iglocska]

* [version] bump. [iglocska]

* [cleanup] removed older revision of upgrade script. [iglocska]

### Fix

* [metafield limitation] fixes. [iglocska]

  - correctly show error messages on user creation when limits are hit
  - fixed a bug that cause users from being uncreatable even due to a hit limitation, even if the current user wouldn't influence said limitation

* [community admin] fixes. [iglocska]

* [ACL component] fixes. [iglocska]
