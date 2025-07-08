# Baited by a QR Code: The Rise of QR Phishing

QR codes are everywhere — menus, check-ins, parking, deliveries. 
But that black-and-white square can **hide a trap** just as easily as a URL.

Welcome to the growing threat of **QR Code Phishing (a.k.a. "Quishing")**.

---

## Why QR Codes Are Dangerous

- Users **can’t see the URL** before scanning
- They bypass email filters — it’s just an image
- QR scanning often happens on **mobile**, where it's harder to inspect links

Combine this with a fake login page and you’ve got a **credential harvesting goldmine**

---

## Real Examples of QR-Based Phishing

| Attack Type           | What It Looks Like                             | Result                           |
|------------------------|------------------------------------------------|----------------------------------|
| Email with QR       | “Scan to verify your Microsoft login”          | Opens phishing page on mobile    |
| Poster in hallway   | “Mandatory Security Training – Scan to Begin”  | Takes you to fake login portal   |
| Delivery Scam       | “Scan to track your package” on fake label     | Requests login or payment info   |
| Business Cards      | “Scan for contact info”                        | Silent redirect to fake portal   |

In recent campaigns, QR phishing emails targeted Office365 and banking users — with **no links in the body**, just a QR image.

---

## Why It Works

- Trains users to “scan everything” 
- Happens on **phones**, which have fewer defenses 
- Looks **legitimate**, especially if printed or placed in public

---

## Red Flags to Watch For

| Clue                         | What It Suggests                         |
|------------------------------|------------------------------------------|
| Email with only a QR code | Bypassing link scanners — likely phishing |
| Random poster with QR      | Could be rogue or tampered               |
| Shortened or masked URLs  | Hard to verify where it leads            |
| Immediate login prompt    | Attackers harvesting mobile credentials  |
| Payment or login request  | QR links shouldn’t ask for sensitive data immediately |

---

## Defending Against QR Phishing

✅ **Don’t scan QR codes** from:
- Emails or chat apps unless confirmed safe
- Posters in public or shared spaces
- Business cards from unknown vendors

✅ On mobile:
- **Long press** the link after scanning to preview the URL
- **Check the domain** — especially for login or payment prompts

✅ On corporate devices:
- Use an **endpoint protection app** that inspects mobile traffic
- Block QR-code-triggered domains not whitelisted

✅ Train users with **real examples** — run monthly “Spot the Fake” exercises with fake vs real QR posters or emails

---

## Quick Awareness Campaign Idea

> Poster Title: “🕵️ Can You Spot a Fake QR Code?”

Design 2–3 posters:
- One with a safe, internal link
- One with a misspelled domain (e.g., `micr0soft-login[.]com`)
- One that leads nowhere (404)

Ask employees to **spot the suspicious one** 
→ Reinforce: *“Don’t trust the code. Check the link.”*

---

## TL;DR: QR Phishing Cheat Sheet

- [ ] Don’t scan QR codes from untrusted sources 
- [ ] Always preview the link **before tapping** 
- [ ] Avoid logging in or paying through QR-scanned links 
- [ ] Check for **short links, weird domains, or typos** 
- [ ] Report suspicious QR posters or emails to security 

---

That little black-and-white square might hide a full-blown attack chain.

➡️ Next up: [How to Report a Phish — Internally and Externally](./how_to_report_phishing.md)
