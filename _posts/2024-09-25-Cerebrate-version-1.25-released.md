---
title:  Cerebrate version 1.25 released with improvements and bugs fixed
tags: release 
---
### Cerebrate v1.25 Release Notes (2024-09-25)

We are excited to announce the release of Cerebrate v1.25! This update includes several new features, enhancements, and bug fixes to improve the overall experience.

#### New Features:
- **UI Enhancements**: Country flags have been added in the following sections:
  - Organisations: /organisations/[index/view]
  - Users: /users/[index/view]  
  _Contributed by Sami Mokaddem_

#### Changes:
- **Docker README**: Updated PHP version.  
  _Contributed by Sami Mokaddem_
- **User Permissions**: Refined permission limitations for organisations on the /users/add page.  
  _Contributed by Sami Mokaddem_
- **Bookmarks**: Improved the handling of malformed content, ensuring the system fails gracefully instead of throwing server errors (500s).  
  _Contributed by iglocska_

#### Fixes:
- **Permission Limitations**: Corrected the display of the number of permission limitations for org_group_managers when an organisation they manage lacks users.  
  _Contributed by Sami Mokaddem_
- **User Filtering**: Added ACL entries for the filtering modal on the users' index page.  
  _Contributed by Sami Mokaddem_
- **UI Fixes**: Adjusted the search dropdown width to prevent overflow on large result sets, addressing issues raised by @gallypette and @adulau.  
  _Contributed by Sami Mokaddem_
- **Group Admin**: Resolved a DatabaseException occurring when a group-admin condition included an empty list of values.  
  _Contributed by Sami Mokaddem_
- **Bookmarks**: Added additional error handling for malformed bookmark entries.  
  _Contributed by iglocska_

#### Other:
- Several merges from `main` and `develop` branches to keep the codebase up-to-date.  
  _Contributed by Sami Mokaddem, iglocska, Andras Iklody_

This release strengthens the stability and functionality of Cerebrate. Thanks to all contributors for their valuable input!

