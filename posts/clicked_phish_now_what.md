# I Clicked a Phishing Link — Now What?

It happens. One rushed moment, one convincing email — and suddenly, you’ve clicked a phishing link or entered your credentials on a fake site.

**This guide is here to help. No panic. Just action.**

---

## First, Stop Everything

Did you:
- Click a suspicious link?
- Enter your password on a fake login?
- Download or open an attachment?
- Approve an MFA prompt you didn’t initiate?

If yes to any of the above, follow the steps below **immediately**.

---

## Step 1: Change Your Passwords

Change the password for:
1. The **compromised account** (e.g., Office365, Gmail)
2. Any other accounts where you **reuse that same password** 
   (Yes, attackers try the same combo on multiple platforms)

✅ Use a **strong, unique password** 

✅ Use a **password manager** if possible

---

## Step 2: Enable or Reconfigure MFA

If your account didn’t already have **Multi-Factor Authentication**:
- **Turn it on** ASAP

If you already had MFA and still got phished:
- Review MFA devices authorized
- Remove old/unknown devices or backup methods

If the attacker harvested your **MFA token via proxy**, they may have already gained access.

---

## Step 3: Don’t Reuse the Link or Revisit the Page

Don’t:
- Click the same link again
- Try to “test” the fake page
- Forward the link without warning

✅ Instead, copy the URL and share it with your **IT/Security team** or **phishing report address**

---

## Step 4: Scan Your Device

If you downloaded anything:
- Run a **full antivirus/anti-malware scan**
- Disconnect from the internet if you suspect active malware
- Check your **Downloads**, **Temp folders**, and **Startup items**

For corporate machines, notify IT to perform deeper forensics if needed.

---

## Step 5: Report It

| Where to Report              | Who Should You Tell                      |
|-----------------------------|-------------------------------------------|
| Company phishing team    | If on a work device or account           |
| `reportphishing@apwg.org` | For public scams (PayPal, Amazon, etc.) |
| Gmail/Outlook “Report”   | Use built-in phishing reporting features |
| Security platform logs  | If EDR/SIEM is in place, tag suspicious behavior |

**The sooner you report it, the more likely others can be warned**.

---

## Step 6: Monitor for Unusual Activity

- Unexpected logins from unknown devices?
- New MFA requests or security emails?
- Password reset requests you didn’t make?

✅ Check:
- Login history (Google, Microsoft, etc.)
- Email forwarding rules (attackers often exfil this way)
- Recent activity in cloud drives or inboxes

---

## Step 7: Don’t Feel Embarrassed

You are **not alone** — even seasoned IT pros click well-crafted phishing links.

What matters is:
- **Speed of response**
- **Transparency**
- **What you learn from it**

---

## TL;DR Recovery Checklist

- [ ] Changed all affected passwords 
- [ ] Enabled or reset MFA 
- [ ] Scanned device for malware 
- [ ] Reported the phishing attempt 
- [ ] Checked login activity & email rules 
- [ ] Warned team/IT/security if applicable 

---

## Prevention Moving Forward

- Use a **password manager** 
- Always **hover over links** before clicking 
- Never enter credentials from a link — **go to the site manually** 
- Verify MFA requests — deny unexpected ones 
- Don’t scan QR codes from posters or unknown emails

---

Got phished once? That makes you **more prepared than someone who hasn’t**.

➡️ Next up: [Why MFA Isn't Foolproof — But Still Saves You](./why_mfa_matters.md)
