---
title: Cerebrate v1.19 released with several usability / functionality fixes 
tags: release 
---

## Cerebrate v1.19 released with several usability / functionality fixes

v1.19 is a maintenance release with fixes and improvements mostly based on the feedback of the CSIRT-Network and ENISA.

### New

- Added session handling related settings

### Fixes

- Keycloak metafield sync fixed
- Keycloak user modification/view issues when more than 100 users were enrolled due to a built in pagination limit in Keycloak
- User enrollment fixes
- Settings fixes
   - Correctly handle the boolean settings such as debug
   - Correctly display numeric settings
   - Ensure that the settings are loaded correctly
- Prevent the saving of an invalid key expiration (either for dates in the past or altogether invalid dates that were cast to indefinite expiration)
- Group admin fixes
  - Group admins can now properly enroll users for organisations other than their own that they manage
  - Group admins can now modify organisation metadata for all of their managed organisations
  - UI fixes to properly reflect what a group admin can do
  - Pagination issues fixed across the board
    - hard limit of 100 elements /page relaxed

### Changes

- Encryption key improvements
  - Reworked UI
  - Fixes to the search interface (search by owner org or individual)
- Various search improvements
  - affected scopes include organisations, users, authentication keys
- Backport and alignment of the MISP3 CRUD component

