# Lab 01: Brute Force Detection - COMPLETED ✅

**Date:** 23-Nov-2026
**Attack:** I simulated a brute force attack by entering wrong passwords 4 times.
**Detection:** Windows Event Viewer -> Windows Logs -> Security -> Filter Event ID 4625
**Result:** Found 4x Event ID 4625, Audit Failure, Task Category: Logon, at 1:33 AM - 1:34 AM

**What This Means:** Event 4625 = Failed Logon. Multiple 4625s in 1 minute = Brute Force pattern.
**SOC Response:** 1. Block source IP, 2. Lock account after 5 failures, 3. Alert user, 4. Enable MFA
**MITRE ATT&CK:** T1110 - Brute Force

**Evidence:** Screenshot shows 4 Audit Failures with Event ID 4625.
<img width="1345" height="710" alt="Screenshot 2026-11-23 015005" src="https://github.com/user-attachments/assets/d817e65e-9c69-4352-9474-afecf824db0b" />
