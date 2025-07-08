# How to Report a Phish — Internally and Externally

Spotted a suspicious email? 
Don't delete it. **Report it.**

Timely reporting helps:
- Stop phishing campaigns early
- Alert others in your organization
- Trigger technical defenses (blocklists, domain takedowns)

---

## What Counts as Phishing?

✅ Looks like a real service (e.g. Microsoft, PayPal)  
✅ Asks for credentials, payment, MFA, or file access  
✅ Contains unexpected attachments or links  
✅ Has a weird sender address or urgent tone  
✅ Feels “off” — even if it looks legit  

> If it makes you hesitate, it’s worth reporting.

---

## Internal Reporting (At Work)

### Step 1: Use the “Report Phish” Button (if available)

Most email platforms now have a **one-click reporting button**:
- Outlook: 🐟 “Report Message” → *Phishing*
- Gmail: ⋮ → *Report phishing*

✅ This sends the email to security tools AND your internal team

---

### Step 2: Forward to Security Team or SOC

If there's no report button, forward the email manually.

Include:
- The original **headers and body** (don’t just describe it)
- A note like: “Received this suspicious email today. Didn't click anything.”

---

### Step 3: Don’t Delete Yet

Wait until the security team confirms it. 
They might:
- Analyze the domain or link
- Search for other recipients
- Use the sample in phishing simulations or blocklists

---

## External Reporting (Public Phishing Scams)

If it wasn’t targeted at your workplace, help the broader community by reporting it.

| Targeting                  | Where to Report                                      |
|----------------------------|------------------------------------------------------|
| General phishing/scam     | `reportphishing@apwg.org`                         |
| Gmail account spoofing    | `phishing-report@google.com`                     |
| Microsoft spoofing        | `phish@office365.microsoft.com`                  |
| Facebook/Instagram scams  | https://www.facebook.com/help/2631496237905943   |
| PayPal phishing           | `spoof@paypal.com`                                |
| SMS/text scams (AU 🇦🇺)    | https://www.acma.gov.au/report-sms-scam          |

📎 Include the **original message as an attachment** (if possible), not just a forward.

---

## What Happens After You Report

Security teams or providers may:
- Block the domain or sender
- Submit the phishing page for takedown
- Notify other users or update training content
- Add the sample to **threat intel feeds**

---

## Reporting = Defense

The faster you report:
- The faster malicious infrastructure gets shut down
- The fewer people fall for it
- The more data defenders have to **improve detection and response**

---

## TL;DR: How to Report a Phish

- [ ] Don’t delete suspicious emails — **report them**
- [ ] Use the “Report” button if your mail platform supports it
- [ ] Forward to internal SOC/security team with headers intact
- [ ] For public scams, send to `reportphishing@apwg.org` or vendor-specific address
- [ ] Don't shame — encourage a culture of quick reporting

---
 
➡️ Next up: [Security Hygiene 101 — The Digital Basics Everyone Forgets](./security_hygiene_101.md) OR ⬅️ [Return to Blog Index](../index.md)
