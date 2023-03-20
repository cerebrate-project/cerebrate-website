---
title: Cerebrate 1.13, including new features, improvements and bug fixes. 
tags: release 
---

We are pleased to announce the immediate availability of Cerebrate 1.13, including new features, improvements bug and security fixes.

We strongly recommend Cerebrate users to update to this latest version.

## v1.13 (2023-03-13)

### New

* [metaTemplateNameDirectory] Added index to see the known template and their associated saved meta-templates. [Sami Mokaddem]

* [user:permissionLimitation] Added current permission status while in `add` or `edit` context. [Sami Mokaddem]

  Also moved the notification key from meta-fields to meta-template-fields

* [element:tagsField] Added support of editable based on passed configuration. [Sami Mokaddem]

* [ui:formInfo] Rafactored formInfo and added support of field description. [Sami Mokaddem]

  Can be done by using the `tooltip` key on the field configuration

* [crud:filter] Added support of IN searches using dropdown. [Sami Mokaddem]

* [component:CRUD] Added support of IN condition when filtering index. [Sami Mokaddem]

### Changes

* [version] bump. [iglocska]

* [meta-template:index] Added link to metaTemplateNameDirectory. [Sami Mokaddem]

* [metaTemplate:update] Gracefully handle case when template on disk is not readable. [Sami Mokaddem]

* [ui:select2] Added CSS file relying on BS variables instead of default theme hardcoded values. [Sami Mokaddem]

* [helper:bootstrap] Make sure to output the value even if it's a `0` [Sami Mokaddem]

* [settings:cerebrate] Improved check before saving debug level. [Sami Mokaddem]

* [component:CRUD] Added `afterFind` support in add. [Sami Mokaddem]

* [user:permissionRestriction] Move check from beforeSave to ApplicationRule. [Sami Mokaddem]

* [component:CRUD] Include meta-template before calling `afterFind` [Sami Mokaddem]

* [tags:org/individual] Relaxed ACL on tagging. [Sami Mokaddem]

  - Before only `site_admin` could add tags.
  - Now `org_admins` can add tags for their orgs and individuals
  - Regular users can self manage their own individual tag

* [encryptionKeys:beforeSave] Updated ACL to disable management of keys for regular orgs. [Sami Mokaddem]

* [encryptionKey] Made key searchable with substring strategy. [Sami Mokaddem]

* [organisations:add] Added notice about UUID reuse. [Sami Mokaddem]

* [helper:bootstrap] Added support of ID option. [Sami Mokaddem]

* [organisations] nationality field renamed to country. [iglocska]

  - UI display only so far
    - want to maintain alignment with MISP, might change in the future
  - filtering still calls it nationality
  - API still calls it nationality

* [roles:index] Only show `add role` button for users having ACL access. [Sami Mokaddem]

* [authkeys:add] Select logged-in user by default. [Sami Mokaddem]

* [audit:filter] Made request_action a multiple search. [Sami Mokaddem]

### Fix

* [meta-template:update]  Typo in variable name. [Sami Mokaddem]

* [elements:dropdownField] Always attach select2 to the body. [Sami Mokaddem]

* [individuals:delete] Gracefully catches deletion of individuals associated to a user. [Sami Mokaddem]

* [acl:metaTemplate] Added missing entry. [Sami Mokaddem]

* [individuals:canEdit] Changed function from public to private. [Sami Mokaddem]

* [elements:bootstrapTabs] Removed unused options. [Sami Mokaddem]

* [elements:metaTemplateForm] Restored error container in the form. [Sami Mokaddem]

* [element:metafields_panel] Correct usage of notices for bootstrap/listTable. [Sami Mokaddem]

* [individual:getValidToEdit] Restricted ACL to prevent one org_admin to edit another from the same org. [Sami Mokaddem]

* [authkey:add] Forced `expiration` field to use datetime UI component. [Sami Mokaddem]

  Fix #145

### Other

* Merge branch 'develop' [iglocska]

* Merge branch 'develop' into main. [Sami Mokaddem]

* Merge branch 'develop' of github.com:cerebrate-project/cerebrate into develop. [Sami Mokaddem]

* Merge branch 'main' into develop. [iglocska]

* Security: [authkey:add] Restrict creation of API keys for users in the same org and for other org_admins. [Sami Mokaddem]

## Shout outs

Thanks to all contributors as well as all users that have let us know about issues, improvement ideas and generally sanity checking what we do. 

A huge [thank to the EC](https://www.enisa.europa.eu/news/enisa-news/open-platform-and-tools-to-facilitate-the-collaboration-among-computer-security-incident-response-teams) for the co-funding for the development of Cerebrate under "Connecting Europe Facility – Cybersecurity Digital Service Infrastructure Maintenance and Evolution of Core Service Platform Cooperation Mechanism for CSIRTs – MeliCERTes Facility” (SMART 2018/1024) contract.

