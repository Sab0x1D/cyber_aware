# BEC Payroll Redirection Attack Flow

Payroll redirect scams are one of the simplest, but most damaging forms of BEC.  
An attacker sends HR a request to “update my salary deposit details.” It works far more often than it should.

---

## What It Looks Like

A typical flow:

1. HR receives an email from “employee.name@company-email.com” (spoofed or compromised)  
2. The email requests to update their bank details “effective immediately”  
3. New bank account is attacker-controlled (often prepaid cards or money mules)  
4. Payroll goes through, but the employee never sees it  
5. Weeks pass before the fraud is discovered  

---

## How the Email Is Crafted

Attackers use personal tone, short language, and urgency. Examples:

> “Hi [HR], I recently changed banks, can we update my direct deposit for this pay cycle?”  
> “Let me know what info you need. I’d prefer to do this over email since I’m in meetings all day.”  

Often, they use lookalike addresses if they don’t have direct access.

---

## Variants and Escalations

- Some attackers start by asking: “How do I update my salary details?” before launching the real fraud  
- Others request PDF forms, fill them out, and send them back, making it look more legitimate  
- Multi-stage versions include fake follow-ups from "supervisors" confirming the update  

---

## Preventing Payroll Redirect Scams

- Never accept banking change requests over email without second-channel verification  
- Use a standardized process for all banking updates, like a secure HR portal  
- Alert HR/payroll teams to these tactics and how to verify requests  
- Monitor for impersonation domains of internal users  

---

## TL;DR: Payroll Redirect Flow

- [ ] HR receives a fake request to change salary deposit info  
- [ ] New details are attacker-controlled  
- [ ] Payment goes through to the wrong account  
- [ ] Employee never receives their pay  
- [ ] Always use a second channel to verify  
- [ ] Secure HR portals eliminate this risk  

---

➡️ Up next: [BEC Detection Playbook for SMBs](./bec_detection_playbook.md) OR ⬅️ Return to Blog Index: [../index.md](../index.md)
