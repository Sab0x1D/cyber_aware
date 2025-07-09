# BEC & Invoice Fraud Explained

Business Email Compromise (BEC) is one of the most financially damaging cyber threats.  
It doesn't rely on malware or exploits — just trust, timing, and a well-crafted email.

This post explains how BEC works, especially through invoice fraud and impersonation tactics, and how to spot it before money leaves the account.

---

## What Is BEC?

BEC is a targeted social engineering attack where cybercriminals impersonate a trusted party — usually a CEO, CFO, or vendor — to trick employees into:

- Sending payments to attacker-controlled bank accounts  
- Changing payroll details  
- Sharing sensitive financial data  

Unlike phishing, BEC emails are often free of links or malware. They’re clean, convincing, and personalized.

---

## Common BEC Variants

1. **CEO Fraud / Executive Impersonation**  
   A spoofed or lookalike email from the CEO requests an urgent wire transfer or sensitive information — often during holidays, weekends, or off-hours.

2. **Vendor Invoice Fraud**  
   Attackers compromise or mimic a vendor’s email and send a modified invoice with new payment details.  
   The victim believes it’s a real invoice from a known supplier.

3. **Payroll Redirect**  
   HR or finance receives a request to update bank account details for salary payments.  
   The new account is controlled by the attacker.

4. **Compromised Email Thread Hijack**  
   An attacker gains access to a real vendor or executive mailbox and replies inside a legitimate ongoing thread — usually with a fake invoice or bank change.

---

## Multi-Staged BEC Attacks

Some of the most convincing BEC frauds are **multi-stage operations** — drawn out over days or weeks to avoid suspicion.  
Attackers mimic real business workflows and slowly build trust before delivering the final fake payment request.

### What It Looks Like:

1. **Initial Vendor Compromise**  
   The attacker gains access to a vendor's real mailbox and monitors communication.

2. **Thread Monitoring or Subtle Interjection**  
   They observe invoice or project-related conversations without interacting — or quietly reply with neutral questions to avoid alerting the target.

3. **Staged Invoice Delivery**  
   An attacker-controlled email sends an invoice **matching expectations** — same amounts, same timing — but with altered bank details.

4. **Reinforcement from a "Supervisor"**  
   A second spoofed email may follow from a fake finance or executive address confirming the payment change is approved.

5. **Urgent Follow-Up Nudges**  
   If the victim hesitates, the attacker pressures with urgency: “Payment is overdue — client project will be delayed unless settled today.”

### Why It Works:

- The invoice appears expected and matches known context  
- Attackers use real branding, footers, and writing tone  
- Multiple emails add credibility  
- Timing aligns with real transactions

---

## Real-World Example: Vendor Scam

A finance team receives this email:

> Subject: Invoice Payment – Past Due  
>  
> Hi team,  
>  
> Attached is our latest invoice for services rendered last quarter. Please note we've updated our banking details due to an audit.  
>  
> Let us know once processed.  
>  
> Regards,  
> Jane M.  
> Accounts — [TrustedVendor]  

The domain name might be a perfect spoof, or the attacker might be replying from the vendor’s actual account.

The victim processes the payment to the attacker’s account, believing it’s real.

---

## Red Flags to Watch For

- Unexpected request to **change banking details**  
- Urgent tone or timing pressure  
- Slightly altered sender address (e.g., jane@trusted-vend0r.com)  
- Reply appears inside a legitimate thread — but invoice file was never sent before  
- Lack of links or signatures that would normally be present  
- Request made outside business hours or by someone who doesn't normally initiate payments  
- Follow-up emails pushing urgency without technical confirmation  

---

## Prevention and Mitigation

- Always verify **banking changes via a separate channel** (phone call, known contact, not by replying)  
- Implement **payment verification workflows** — dual approvals for any account changes or large transfers  
- Use **mailbox rule alerts** to detect auto-forwarding or filtering rules (common in compromised accounts)  
- Train staff to **recognize tone manipulation** and trust exploitation  
- Monitor for **lookalike domains** targeting your business or vendors  
- Enable **DMARC, SPF, and DKIM** for email authentication  

---

## What To Do If You Suspect BEC

- Do not reply — verify the request through known-good channels  
- Inform your security or IT team immediately  
- Contact the bank if a transfer occurred — fast action may allow a recovery  
- Report the incident to your country’s cybercrime unit or financial fraud division  

---

## TL;DR: BEC Invoice Fraud

- [ ] No links or malware — just social engineering  
- [ ] Executive or vendor impersonation is common  
- [ ] Email asks for payment or banking change  
- [ ] May be multi-staged, spread over several emails  
- [ ] Always verify requests via a second channel  
- [ ] Watch for domain spoofing and thread hijacking  
- [ ] Dual-approval or callback verification can stop it  
- [ ] Report immediately if something feels off  

---

➡️ Up next: [Vendor Hijack Case Study](./bec_vendor_hijack_case_study.md) OR ⬅️ Return to Blog Index: [../index.md](../index.md)
