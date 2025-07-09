# BEC Vendor Hijack Case Study

A vendor email account gets compromised. Days or weeks later, the attacker strikes, right from inside the vendor's real inbox, replying in a genuine thread.

This post walks through a real-world case study of vendor email hijack, explaining how it unfolded and how it could have been caught.

---

## Background

A mid-sized business received an invoice via email, from a long-standing vendor, for services recently completed.  
The invoice matched the expected amount and timing. But the bank details had changed.

They paid it.

Only weeks later did the real vendor reach out asking why the invoice hadn’t been paid.

---

## What Actually Happened

The attacker had compromised the vendor’s Microsoft 365 email account using stolen credentials.  
Once inside, they:

- Set up forwarding rules to monitor finance-related conversations  
- Waited silently for an invoice to be generated  
- Modified the PDF with new bank details  
- Sent the invoice from the real vendor email, inside the actual email thread  
- Followed up days later to “remind” the recipient to process the payment  

It was clean. There were no red flags. No malware. Just trust.

---

## Technical Clues Missed

- A forwarding rule in the vendor’s mailbox quietly sent a copy of all emails to a Gmail address  
- The invoice file was last edited from a non-corporate IP  
- SPF/DKIM/DMARC failures weren’t enforced on the recipient's side  
- No second-channel verification occurred for the banking change  

---

## How It Could Have Been Caught

- Finance team should have verified any banking change over phone or known contact  
- The slightly unusual filename on the invoice (e.g., “inv_final_update_v2.pdf”) might’ve raised suspicion  
- Logging into the vendor portal or past email trail would show a different account used previously  

---

## Lessons Learned

- Even legitimate threads can be poisoned after a breach  
- You must trust **the process**, not just the sender  
- Quiet email rule monitoring is a strong indicator of compromise  
- Every finance team should have a checklist before honoring payment changes  

---

## TL;DR: Vendor Hijack Case Study

- [ ] Invoice sent from a real vendor account  
- [ ] Payment details were altered by the attacker  
- [ ] Email thread was genuine, but manipulated  
- [ ] Forwarding rules helped attackers monitor  
- [ ] Payment verification checklist would have stopped it  
- [ ] Post-incident, vendor needed to reset credentials and rules  

---

➡️ Up next: [Payroll Redirect Flow](./bec_payroll_redirect_flow.md) OR ⬅️ Return to Blog Index: [../index.md](../index.md)
