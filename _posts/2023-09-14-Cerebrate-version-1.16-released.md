---
title: Cerebrate version 1.16 released released including new features and improvements 
tags: release 
---

## Cerebrate version 1.16 released including new features and improvements

### Organisation Group management added

With the release of 1.16, we have introduced the new concept organisation groups, an administrative layer sitting on top of organisations, allowing designated group administrators to manage a set of organisations. 

Whilst this feature comes as a newly requested feature submitted by ENISA for managing the European CSIRT network, we already see a host of other possibilities for taking advantage of it, ranging from virtual organisation grouping to managing larger sharing communities with self-reliant sub-groups.

In essence, the new feature allows for the creation of sub communities with a degree of self-management, so if you would like to enroll say an ISAC or other sectorial / national group in your community, this can greatly ease the burden of user management on the site administrators by delegating the task to entrusted parties within the sub communities.

Our experience with both MISP and with Cerebrate has shown that contrary to the most common immediate observaions of a potential risk coming from diluting administrative responsibilities, it actually achieves the opposite, by allowing for a smoother, self-service management of not only user enrollment, but also rotating out user accounts and general auditing and life-cycle management of user accounts.

As a site administrator, simply create a new group:

![image](https://github.com/cerebrate-project/cerebrate/assets/3668672/2273b6ee-4ed3-4ea1-90b9-0acf4f76e0e7)

Add administrator(s) to the group to allow for self-management:

![image](https://github.com/cerebrate-project/cerebrate/assets/3668672/e69b1ada-d62a-4ad6-b276-c09a57d9105d)

Start adding organisations to the group:

![image](https://github.com/cerebrate-project/cerebrate/assets/3668672/eb6565b7-03a8-41f6-bd60-be448aafbb84)

Once done, the desginated group administrator can start managing the users of the listed organisations.


### Changes

* [users:acl] Improved waterfall model for CRUD operation and updated UI to reflect them. [Sami Mokaddem]

* [ui] Improved reflection of ACL logic in the UI for OrgGroups, Organisations and individuals. [Sami Mokaddem]

* [VERSION] bump. [iglocska]

* [alignments:acl] Reflected ACL logic from individuals to alignments. [Sami Mokaddem]

* [users:edit] Allow users to self edit. [Sami Mokaddem]

* [user-settings:edit] Prevent assigning a setting to another user. [Sami Mokaddem]

* [command:summary] Added data about the modified entity. [Sami Mokaddem]

* [navigation:tags] Updated UI to reflect users' permissions. [Sami Mokaddem]

* [navigation:individuals] Only show edit and deletion buttons if users are allowed to do it. [Sami Mokaddem]

* [genericElements:numberOfElement] Added parameter to show or not the `show all` option. [Sami Mokaddem]

* [ACL:tags] Relaxed ACL on tags for index and view pages. [Sami Mokaddem]

* [ACL:individual/add] Allow `org-admin`s to create new individuals. [Sami Mokaddem]

### Fix

* [ACL] group admins can view users in their group. [iglocska]

* [internal] fixed the function checking if a user belongs to the current User's managed org group. [iglocska]

* [acl:canEditUser] Typo in table name. [Sami Mokaddem]

* [OrgGroups:checkIfGroupAdmin] Consider site_admins as group admin. [Sami Mokaddem]

* [strict typing] Made Sami's frankenstein setup happy. [iglocska]

* [temp] ACL function built up. [iglocska]

* [ACL] fixes. [iglocska]

* [org admins] should be able to edit the org. [iglocska]

* [individual:edit] Select individuals based on their id and not their user_id. [Sami Mokaddem]

* [navigation:CRUDAction-auditlogs] Make ordering by created field unambigous and hide audit button to non-admin users. [Sami Mokaddem]

* [userSettings:add] Aded check to avoid duplicated setting for the same user. [Sami Mokaddem]

* [mailinglist:ACL] Fixed bug in ACL check for access. [Sami Mokaddem]

