# MFA Bypass Case Studies: Real-World Attacks

Multi-Factor Authentication (MFA) **dramatically reduces risk**, but it's not unbeatable.

This post explores real examples of MFA bypass in the wild — how attackers pulled it off, and what we can learn.

---

## Case 1: Evilginx2 Phishing Proxy

> **Target:** Corporate O365 Accounts 
> **Vector:** Phishing Email with Fake Microsoft Login 
> **Method:** Reverse Proxy + Real-Time MFA Capture

The phishing link pointed to an **Evilginx2** server, acting as a man-in-the-middle between user and real Microsoft login.

- The victim enters their credentials
- The real Microsoft login is loaded behind the scenes
- The MFA token is passed through
- Attacker captures a valid session cookie (authentication token)

**Bypassed MFA completely**, without needing password reuse or device access

**Defensive Tip:** 
→ Use **device-bound sessions**, **conditional access policies**, and **phishing-resistant MFA** (e.g., FIDO2 keys)

---

## Case 2: MFA Fatigue Attack on Uber (2022)

> **Target:** Internal Uber Systems 
> **Vector:** Compromised credentials + repeated push notifications 
> **Method:** MFA fatigue + social engineering

The attacker spammed the user with push requests from the Authenticator app.

Eventually, the user clicked "Approve" to stop the annoyance.

- This granted access to internal systems
- Attacker reportedly contacted the user pretending to be IT to "confirm the login"

Successful access **without needing password cracking or malware**

**Defensive Tip:** 
→ Use **number matching**, **user prompt verification**, or **rate-limiting** MFA attempts

---

## Case 3: SIM Swap + SMS MFA Intercept

> **Target:** Crypto wallet account 
> **Vector:** Social engineering telco to port victim's number 
> **Method:** SIM Swap → Intercept SMS MFA

The attacker convinced the victim’s phone provider to **reassign the number** to a SIM card under their control.

- Reset password via email
- Received the **MFA code via SMS**
- Logged into and drained the crypto wallet

The attacker never touched the device or breached an app

**Defensive Tip:** 
→ Never use SMS for critical accounts 
→ Use **hardware-based MFA**, and ask your telco to add **port-out protection**

---

## Case 4: QR Code Login Hijack (Corporate Poster Bait)

> **Target:** Internal employees 
> **Vector:** Malicious QR code on break room poster 
> **Method:** QR leads to fake Microsoft login

Poster advertised a “mandatory training portal” with a QR code.

- Mobile device opens a fake Microsoft login page
- Victim logs in + enters MFA code
- Attacker relays credentials in real-time

Fully bypassed MFA from a **trusted-looking internal source**

**Defensive Tip:** 
→ Treat **QR codes as potential phishing vectors** 
→ Restrict login access from unknown devices + monitor **geolocation anomalies**

---

## Key Lessons

| Tactic                   | MFA Stolen or Bypassed?          | Mitigation Strategy                                |
|--------------------------|----------------------------------|----------------------------------------------------|
| Evilginx2 Proxy          | ✔️ Session token stolen           | Use FIDO2 or device-bound tokens                   |
| Push Fatigue             | ✔️ User approval tricked          | Enable push verification or number matching        |
| SIM Swap                 | ✔️ SMS code intercepted           | Avoid SMS; use app-based MFA or physical keys      |
| QR Phishing              | ✔️ Real-time MFA relay            | Awareness + login monitoring + geo restrictions    |

---

## TL;DR: Make MFA Resilient

- [ ] Use **phishing-resistant MFA** (hardware keys, FIDO2) 
- [ ] Avoid SMS and email recovery flows for critical accounts 
- [ ] Don’t blindly approve MFA prompts — verify the login attempt 
- [ ] Monitor device, IP, and session activity for anomalies 
- [ ] Educate users about **proxy phishing and MFA fatigue** 

---

MFA isn't dead — but like passwords, it **must evolve** to stay effective.

➡️ Next up: [Building a Human Firewall — Training Non-Technical Staff](./human_firewall_training.md) OR ⬅️ [Return to Blog Index](../index.md)
