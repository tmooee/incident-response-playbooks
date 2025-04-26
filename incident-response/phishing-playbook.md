# 🛡️ Incident Response Playbook – Phishing Email

## 🎯 Objective
Contain and mitigate phishing attacks that aim to steal credentials or deliver malware.

---

## 🧾 Detection

- User-reported phishing email
- Suspicious link or attachment in email
- Login page mimicking internal systems

---

## 📊 Log Sources

- Email security gateway
- Endpoint telemetry (EDR)
- DNS and proxy logs

---

## 🔍 Validation Steps

- Analyze headers, links, and attachments
- Use threat intel to verify domains/IPs
- Check if any users clicked or entered credentials

---

## 🛑 Containment

- Quarantine email in all inboxes
- Block sender/domain/IP
- Notify affected users

---

## 🧼 Eradication

- Remove downloaded payloads
- Scan endpoints for malware or persistence

---

## 🔄 Recovery

- Reimage infected systems if needed
- Reset passwords for impacted accounts

---

## 📣 Communication

- Inform users of campaign and red flags
- Share indicators with threat intel team

---

## 📘 Lessons Learned

- Update phishing training
- Improve email filtering or SPF/DKIM/DMARC
