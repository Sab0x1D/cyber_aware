# Fake Login Portals: How Hackers Steal Your Credentials

Phishing emails are often just **the bait**. The real trap? A **fake login page** that looks almost identical to a real one.

Whether it’s your Microsoft account, Google, banking, or even crypto wallets, attackers build pixel-perfect clones to trick you.

---

## What Are Fake Login Portals?

These are **webpages designed to mimic legitimate login pages**, such as:

- `Outlook`, `Microsoft 365`, `Google`, `Dropbox`
- Internal company portals
- Payment gateways or banking sites

They're **usually delivered via phishing emails or malicious QR codes**, and their only job is to **harvest your credentials**.

---

## How They Trick You

| Method                  | What It Looks Like                          | What’s Really Happening                       |
|--------------------------|-----------------------------------------------|------------------------------------------------|
| Email link               | `https://secure.microsoft-login.com`         | A clone site hosted on a malicious domain      |
| QR code poster in café   | “Scan to check in” (linked to `login.mygov.au`) | Loads fake site stealing MyGov credentials     |
| Fake popup in browser    | “Your session has expired. Login to continue” | Injected HTML by malicious browser extension   |
| MFA prompt               | “Enter code to verify” after fake login       | Attacker relays real login request via proxy   |

---

## Real Example Breakdown

> Subject: ⚠️ Outlook Security Alert – Re-authentication Required 
>
> 
> You must re-authenticate your email to avoid account lockout. 
>
> 
> 👉 [Sign In to Outlook](https://login-outlook-authenticate.com) 
>
> 
> – IT Helpdesk

✅ Link **looks close** to real Outlook but it’s off.  
✅ Clicking takes you to a **cloned Outlook login page**.  
❌ Anything you type goes **straight to the attacker**.  

---

## 6 Clues You’re on a Fake Login Page

| Red Flag                    | How to Check                           |
|----------------------------|------------------------------------------|
| URL isn’t quite right   | Should be `https://outlook.office.com`, not `.xyz` or `.login-security.com` |
| No padlock or invalid cert | Click the 🔒 icon — if missing or red, leave immediately |
| Poor grammar or typos   | Legitimate companies don’t make basic mistakes |
| Slight design inconsistencies | Fonts, logos, or spacing look “off” — attackers often miss small details |
| Asked to enter credentials multiple times | Legit portals rarely ask twice unless something failed |
| Loads very slowly or glitches | Often hosted on cheap or slow servers |

---

## How These Sites Are Built

Attackers may use:
- **HTTrack** or **wget** to clone entire login pages
- **JavaScript keyloggers** to intercept input
- **Man-in-the-middle kits** like Evilginx2 or Modlishka to proxy real logins

Goal: **Harvest real usernames, passwords, and even MFA tokens** in real time

---

## How to Protect Yourself

✅ **Always check the domain** — especially on mobile  
✅ Use a **password manager** — it won’t autofill on fake sites  
✅ Enable **MFA**, preferably app-based (not just SMS)  
✅ Don’t scan **random QR codes** from posters, emails, or chat apps  
✅ Report suspicious links to your IT/security team  

---

## Bonus Tip: Hover Test

Before clicking a login link:

- **Desktop:** Hover with your mouse — check the real destination
- **Mobile:** Long-press the link and inspect the URL carefully

If in doubt, **open the login page manually** via your bookmarks.

---

## TL;DR: Fake Login Portal Red Flags

- [ ] URL is slightly off (e.g., `login-outlook-verify.com`) 
- [ ] Site uses HTTP or shows certificate errors 
- [ ] Login looks real but design feels odd 
- [ ] Unexpected login requests from emails or QR codes 
- [ ] You’re asked to enter MFA code right after password 
- [ ] Page doesn’t behave like the real thing (slow, unresponsive)

---

Stay alert. Don’t trust — verify.

➡️ Up next: [What to Do After Clicking a Phishing Link](./clicked_phish_now_what.md) OR ⬅️ [Return to Blog Index](../index.md)
