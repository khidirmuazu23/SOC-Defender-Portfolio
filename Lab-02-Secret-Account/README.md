# Lab 02: Detect Secret Account Creation - Persistence

**Attack:** Attacker created a secret account called hacker123 to maintain access.
**Detection:** Event Viewer -> Security -> Filter Event ID 4720
**Result:** Found 1x Event ID 4720 - A user account was created - Account Name: hacker123
**SOC Response:** 1. Disable the account immediately, 2. Delete it, 3. Check what that account did, 4. Reset admin passwords
**MITRE ATT&CK:** T1136 - Create Account
**Lesson:** A new account appearing at 2 AM when no one is working is a big red flag.

**Evidence:** [Add screenshot of 4720 here]
<img width="1365" height="726" alt="Screenshot 2026-11-23 095400" src="https://github.com/user-attachments/assets/2e2a8125-9cdb-4d0b-b9ed-c2ab3f71d906" />
