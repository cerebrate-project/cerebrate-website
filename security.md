---
layout: article
titles:
  # @start locale config
  en      : &EN       Security 
  # @end locale config
key: page-security
---

# Security Policy

## Reporting security vulnerabilities for Cerebrate or related Cerebrate project repositories

Reporting security vulnerabilities is of great importance for us, as Cerebrate project is used by different security operators and organisations. 

In the case of a security vulnerability report, we ask the reporter to send it directly to [CIRCL](https://www.circl.lu/contact/), if possible encrypted with the following GnuPG key: **CA57 2205 C002 4E06 BA70 BE89 EAAD CFFC 22BD 4CD5**. We usually fix reported and confirmed security vulnerabilities in less than 48 hours, followed by a software release containing the fixes within the following days. 

If you report security vulnerabilities, do not forget to **tell us if and how you want to be acknowledged** and if you already requested CVE(s). Otherwise, we will request the CVE(s) directly.

As one of the critical user-bases of Cerebrate project consists of the CSIRT community, it is our duty to clearly state which bug could be abused and have a security impact on a Cerebrate instance. CVE assignment is performed even for minor bugs suspected of having a security impact. This allows every user with Cerebrate instances set up in their environments to understand which bugs could impact their security.

We firmly believe that, even though unfortunately it is often not regarded as common practice in our industry, being as transparent as possible about vulnerabilities, no matter how minor, is of crucial importance. At Cerebrate Project, we care about the security of our users and prefer to have a high number of published CVEs rather than sweeping some of them under the rug.

## Advisories

- [CVE-2022-25317](https://cvepremium.circl.lu/cve/CVE-2022-25317)
- [CVE-2022-25318](https://cvepremium.circl.lu/cve/CVE-2022-25318)
- [CVE-2022-25319](https://cvepremium.circl.lu/cve/CVE-2022-25319)
- [CVE-2022-25320](https://cvepremium.circl.lu/cve/CVE-2022-25320)
- [CVE-2022-25321](https://cvepremium.circl.lu/cve/CVE-2022-25321)
- [CVE-2023-26468](https://cvepremium.circl.lu/cve/CVE-2023-26468) <= Cerebrate 1.12
- [CVE-2023-28883](https://cvepremium.circl.lu/cve/CVE-2023-28883) -  In Cerebrate 1.13, a blind SQL injection exists in the searchAll API endpoint. 
- [CVE-2023-41363](https://cvepremium.circl.lu/cve/CVE-2023-41363) <= Cerebrate 1.14 - In Cerebrate 1.14, a vulnerability in UserSettingsController allows authenticated users to change user settings of other users.  

## PGP key

~~~~
-----BEGIN PGP PUBLIC KEY BLOCK-----

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
=fKH+
-----END PGP PUBLIC KEY BLOCK-----
~~~~

