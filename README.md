# Archived Repository
This repository has been archived and will no longer receive updates.
It was archived as part of the [Repository Standardization Initiative](https://github.com/chef-boneyard/oss-repo-standardization-2025).
If you are a Chef customer and need support for this repository, please contact your Chef account team.

---

# Windows-DNS-SIGRed

This profile identifies systems that are missing one or more of the required patches to address [CVE-2020-1350, Windows DNS Server Remote Code Execution Vulnerability](https://portal.msrc.microsoft.com/en-us/security-guidance/advisory/CVE-2020-1350).

This profile utilizes InSpec's `describe.one` method to test against the multiple KB's without the need for complex OS version logic. It will also consider the [workaround registry key](https://portal.msrc.microsoft.com/en-us/security-guidance/advisory/CVE-2020-1350#ID0EUGAC) as a success. Please note, InSpec tests the decimal value of the registry key. This test specifies 65280d which equals FF00h.
