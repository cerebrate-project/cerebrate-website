---
title: Cerebrate v1.20 released with various bugs fixed 
tags: release 
---

### New Features

* **Metafield Restrictions:** Not enforced on an edit that doesn't change the state of the offending value.
  - If a user is already over the limit of a restriction, they should still be editable.

### Changes

* **Encryption Keys:** Listed for organizations and individuals on their respective views. (Fixes #167)
* **Dashboard Redirects:** To individual models now sort by modified by default.
  - The dashboard shows new entries, making it logical to sort the list based on changes.
  - Small fix to avoid sanitizing index URLs, ensuring multiple query parameters work correctly.

### Fixes

* **Alignments:** Rules relaxed. (Fixes #164)
  - Site admins can add alignments to anyone.
  - Organization admins can add alignments for their own organization members.
  - Group admins can add alignments for any of their managed organization's members.
* **Authkeys:** Allow for authkeys with no expiration set. (Fixes #169)
* **Authkey Add:** Ensure default to expiration=0 if not provided.
* **Encryption Keys:** Allow for large keys.
* **Setting Cerebrate:** Enforce debug setting to be true or false.

