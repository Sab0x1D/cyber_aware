# Infected USB Case Example — A Physical Attack That Still Works

Despite being one of the oldest tricks in the book, **infected USB drops** are still used in real-world attacks — often successfully.  
This post walks through a real case scenario of how a planted USB device led to full system compromise.

---

## What Is a USB Drop Attack?

Attackers deliberately leave **malicious USB drives** in:

- Office lobbies  
- Parking lots  
- Airports, libraries, or cafés  
- Company restrooms or breakrooms  

These drives are often labeled with something tempting like:

- “2024 Salaries.xlsx”  
- “HR Reports”  
- “Photos”  
- “Confidential”  

The goal? **Curiosity.** Someone plugs it in, and the payload does the rest.

---

## Case Study: “Company Roster.xls” USB

A consulting firm received an envelope addressed to HR. Inside:

- A generic note: “As requested — latest roster export”
- A USB drive labeled `Company_Roster_2024.xls`

An HR staff member plugged it into their Windows PC.

What happened:

1. USB was set to auto-run a hidden `.lnk` shortcut  
2. Shortcut silently launched a PowerShell stager  
3. Malware beaconed out to a remote C2 server  
4. Attacker gained access — credential dump, lateral movement, and domain recon followed within minutes

---

## Why This Worked

- The USB drive looked legitimate  
- Delivered internally (no firewall or email scan involved)  
- Curiosity and urgency — “I better check this now”  
- No USB scanning tools in place  
- Auto-run was enabled for removable media

---

## Prevention Measures

- ✅ Disable **AutoPlay/AutoRun** for all USB and removable drives  
- ✅ Enforce **USB control policies** — allow only approved devices  
- ✅ Train staff: **Don’t plug in unknown USBs** — even from postal mail  
- ✅ Use **endpoint security** tools to scan external devices  
- ✅ Log and alert on execution of `.lnk`, PowerShell, or EXE from USB paths  
- ✅ Provide secure file-sharing alternatives for third parties

---

## TL;DR: Infected USBs Still Work

- [ ] USB drop attacks exploit curiosity  
- [ ] Often paired with shortcut tricks, PowerShell payloads, or HID emulation  
- [ ] Easily bypasses email filters and EDR  
- [ ] Disable AutoRun + train users = huge risk reduction  
- [ ] Never trust a drive you didn’t request  

---

➡️ Up next: [QR Codes in Public Spaces](./qr_codes_in_public.md)  
⬅️ [Return to Blog Index](../index.md)
