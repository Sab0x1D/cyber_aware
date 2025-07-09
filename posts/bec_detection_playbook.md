# BEC Detection Playbook for SMBs

Business Email Compromise is stealthy, targeted, and difficult to detect with antivirus or firewalls.  
For small to mid-sized businesses (SMBs), prevention depends on process and people, not tools.

This post offers a practical playbook to help detect and defend against BEC incidents.

---

## Detecting the Signs of BEC

- Unexpected request to change payment or banking info  
- Emails requesting secrecy, urgency, or “out of band” handling  
- Reply chains that contain files or changes never seen before  
- Unusual email login activity (e.g., logins from foreign IPs)  
- Inbox rules that forward or hide emails  
- Changes to email signatures or reply patterns  

---

## Prevention Is the Best Detection

BEC works because it bypasses technical defenses — so the best detection is **stopping it before it happens**:

- Train finance, HR, and executive assistants on BEC tactics  
- Require secondary confirmation for any banking/account changes  
- Use email banners for external senders  
- Block lookalike domains or alert on near-matches  

---

## What to Log and Monitor

- New inbox rules or auto-forwarding rules  
- Logins from suspicious geolocations  
- Excessive failed logins to finance or executive inboxes  
- Unusual editing metadata in PDFs (different authors, last modified from outside IPs)  
- Sudden removal of MFA on an account  

---

## Building the BEC Response Plan

Every SMB should have:

- A documented payment verification checklist  
- A known-good contact directory for external vendors  
- A process to pause payments if fraud is suspected  
- A recovery protocol (e.g., banking escalation, incident report template, insurance contact)  

---

## TL;DR: Detection Playbook

- [ ] BEC detection relies on behavioral signs  
- [ ] Inbox rules and logins are early indicators  
- [ ] Train staff to question urgent changes  
- [ ] Always confirm payment changes with a call  
- [ ] Build a checklist and a reporting process  

---

⬅️ Return to Blog Index: [../index.md](../index.md)
