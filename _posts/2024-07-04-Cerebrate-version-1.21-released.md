---
title: Cerebrate v1.21 released with various bugs fixed 
tags: release 
---

## v1.21 (2024-07-02)

### New

* [extended logger] added. [iglocska]

  - Added more information about the request to the stack traces
  - logs user name / ID
  - logs request x-forwarded-for

### Changes

* [tag] bumped. [iglocska]
* [permission limitations] free limitation count when user disabled. [iglocska]
  - Thanks to Elisabeth from BSI for reporting it
* [permission limitations] free limitation count when user disabled. [iglocska]

### Fix

* [user add] fixed bug with metafields on new users causing an exception. [iglocska]

