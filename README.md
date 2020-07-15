# Windows-DNS-SIGRed

This profile identifies systems that are missing one or more of the required patches to address CVE-2020-1350, Windows DNS Server Remote Code Execution Vulnerability.

This profile utilizes InSpec's `describe.one` method to test against the multiple KB's without the need for complex OS version logic.
