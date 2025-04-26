# 🛡️ Incident Response Playbook – Brute Force Login Attempts

## 🎯 Objective
Contain and mitigate brute force login activity targeting web apps, VPNs, or internal systems.

---

## 🧾 Detection

- Multiple failed login attempts (HTTP 401, Windows Event ID 4625)
- Spike in login attempts from same IP or user
- Successful login after multiple failures

---

## 📊 Log Sources

- Apache/Nginx logs
- Windows Security logs
- VPN/SSO provider logs

---

## 🔍 Validation Steps

- Confirm high volume of failed logins in short timeframe
- Cross-check with known bad IP reputation databases
- Identify any successful logins post-failure

---

## 🛑 Containment

- Block offending IP address at firewall or WAF
- Disable affected user accounts
- Force password reset + MFA enforcement

---

## 🧼 Eradication

- Verify no persistence mechanisms or lateral movement
- Check for signs of privilege escalation or data access

---

## 🔄 Recovery

- Re-enable accounts with new credentials
- Tune detection rules to reduce false positives

---

## 📣 Communication

- Notify affected users and stakeholders
- Escalate to Tier 2 if account compromise confirmed

---

## 📘 Lessons Learned

- Were detection rules tuned effectively?
- Was MFA enforced where possible?
