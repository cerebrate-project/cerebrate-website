---
title:  Cerebrate version 1.24 released with API improvements Latest 
tags: release 
---

## v1.24 (2024-08-29)

## API improvements

### Improvement of meta field usage via the API

Add/Edit endpoints have been updated to accept a simplified format of metafields for easier integration. Metafields are now passed as a list of objects with 4 required keys (field, value, template_uuid and template_version).

An example for adding a user, along with metafields set is as follows:

```
{
    "individual": {
        "email": "andras.iklody@circl.lu",
        "first_name": "Andras",
        "last_name": "Iklody"
    },
    "username": "andras.iklody@circl.lu",
    "organisation_id": "2",
    "role_id": "3",
    "meta_fields": [
      {
        "field": "perm_misp",
        "value": true,
        "template_uuid": "447ded8b-314b-41c7-a913-4ce32535b28d",
        "template_version": 2
      }
    ]
}
```

### Better error handling

Passing malformed data or not setting the proper media type headers resulted in rather arcane messages, complaining about certain validation errors / missing fields in the provided content. This lead to a fair bit of confusion, so from v1.24 on, if for whatever reason Cerebrate cannot pick up on the contents of a POST/PUT request, it will return a 400 warning the user about malformed / missing post bodies. 

Thanks to [Paweł Pawliński](https://github.com/pp-) for testing the API and providing feedback!

### Alignments and authoring of individuals

In order to shed the frustrations that were up until now caused by org admins / group admins being able to create Individuals, but not to modify them after the fact, we have modified the behaviour altogether. 

Having an alignment to the individual enabled org/group admins to modify individuals and as of v1.24, any individual created by one of them will automatically be aligned with their organisation. This should allow org/group admins to retain authoring right.

### Version and links to the Cerebrate-project resources

We have added a link to both Cerebrate-project's website and the release notes of the current version to a small header text displayed at all times after login, also indicating the currently installed version for easier identification. 
