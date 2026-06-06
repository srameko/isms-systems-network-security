---
layout: section
subtitle: ISO 27001 — Control 8.20
---

# Network Security

---
layout: default
---

# 8.20 Network Security

**A documented network security standard exists**, covering:

- Defined **network zones**
- Allowed **data flows**

The standard must be:
- Understandable
- Up to date
- Actually used in practice

---
layout: default
---

# 8.20 Device Hardening

Network devices must be:

| Requirement | Examples |
|-------------|---------|
| **Hardened** | Minimal services, secure defaults |
| **Updated** | Regular patch cycles |
| **Managed** | Centralised config management |

Applies to **everything with a management interface**:
Firewalls · Routers · Switches · VPN · Printers · Access Points

---
layout: default
---

# 8.20 Network Access

- Network is divided into **security zones**
  - Guest · DMZ · ICS/IoT/SCADA
- Critical systems are:
  - Isolated
  - Protected by stricter rules
- **Device-level authentication** for network access

---
layout: default
---

# 8.20 Remote and Wireless Access

**Remote Access (VPN)**
- Multi-Factor Authentication (MFA) and additional security steps
- Encryption

**Wi-Fi**
- Separate networks for employees and guests
- Access verification

---
layout: default
---

# 8.20 Logging and Monitoring

Key network events must be:
- **Logged**
- **Monitored**

The organisation must be able to:
- Detect suspicious traffic
- Investigate incidents

---
layout: default
---

# 8.20 Cloud vs On-Premise

<div class="icon-grid cols-2">
  <div class="icon-card">
    <div class="icon">☁️</div>
    <div class="label"><strong>Cloud</strong><br/>Same security principles apply — cloud ≠ exception to security</div>
  </div>
  <div class="icon-card">
    <div class="icon">🏢</div>
    <div class="label"><strong>On-Premise</strong><br/>Controls defined and documented, regularly reviewed</div>
  </div>
</div>

<div class="callout warning">
Cloud is not an exemption from security requirements.
</div>

---
layout: default
---

# 8.20 Change Management

Network changes must go through:
- **Change management process**
- Approval workflow
- Rules are **regularly reviewed**

---
layout: default
---

# 8.20 Audit

The organisation must be able to demonstrate:

- Configurations
- Network diagrams
- Logs
- Change records

Security must be **provable and sustainable**.

---
layout: default
---

# 8.20 Metrics

| Metric | Description |
|--------|-------------|
| Device status | How many are up-to-date |
| Logins | Successful vs failed authentication |
| Packet loss | Network health indicator |
| Connected devices | Wired / wireless / guest network count |

---
layout: default
---

# 8.20 Common Problems

<div class="callout warning">
Cloud is often left unmanaged — default settings in place, nobody monitoring
</div>

- Nobody monitoring network activity
- Management interfaces exposed to the internet
- Weak or missing authentication
- Impossible to trace which device caused an incident
