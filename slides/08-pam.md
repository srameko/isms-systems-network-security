---
layout: section
subtitle: ISO 27001 — Control 8.2
---

# PAM / PIM — Privileged Access Management

---
layout: default
---

# 8.2 Privileged Access Rights / Management

Privileged accounts represent the **highest risk** if compromised.

Control 8.2 ensures they are strictly managed, monitored, and used only when necessary.

**In scope:**
- Administrator and system accounts
- Accounts enabling:
  - Configuration changes
  - Software installation
  - User management
  - Access to sensitive data

---
layout: default
---

# 8.2 Privileged Access Rights

Goal: ensure privileged access rights (admin, root, enterprise admin) are granted, used, and managed in a **controlled manner** — reducing the risk of misuse or compromise.

<div class="callout">
In practice, commercial PAM software is typically used: <strong>CyberArk, BeyondTrust</strong> and similar solutions.
</div>

---
layout: default
---

# 8.2 PAM — Core Principles

**Least Privilege**

- Privileged access only for **authorised persons**
- Only for the **minimum necessary time** (request/time-boxed)

**Account Separation**

- Regular user accounts
- Administrator accounts
- In practice: multiple permission tiers (R, RW…)

---
layout: default
---

# 8.2 PAM — Key Requirements

<div class="icon-grid">
  <div class="icon-card">
    <div class="icon">📋</div>
    <div class="label">Formal process for approval, changes, and revocation</div>
  </div>
  <div class="icon-card">
    <div class="icon">📅</div>
    <div class="label">Evidence and regular access review (typically annual)</div>
  </div>
  <div class="icon-card">
    <div class="icon">🔑</div>
    <div class="label">MFA (Passkeys, Push notifications…)</div>
  </div>
  <div class="icon-card">
    <div class="icon">📝</div>
    <div class="label">Logging and monitoring of all privileged activity</div>
  </div>
</div>

---
layout: default
---

# 8.2 PAM — Roles and Responsibilities

| Role | Responsibility |
|------|---------------|
| **Management** | Approves policies and exceptions |
| **Security** | Controls and audits privileged accounts |
| **IAM** | Manages privileged accounts |
| **Users** | Responsible for safe use of their access |

---
layout: default
---

# 8.2 Do Nots

**Common Examples**

<div class="callout warning">
Forgotten or unrecorded accounts with admin access (including Shadow IT)
</div>

- No logging or monitoring
- No MFA
- Sharing credentials for generic accounts like `admin42@org.cz`
- Weak passwords

**Resulting Risks**

- Data loss
- Integrity compromise
- Availability disruption

---
layout: default
---

# PAM — Summary

**Privileged Access Management** covers:

- Management and security of privileged accounts (admin, root, service accounts)
- Restricting access according to **least privilege**
- **Just-In-Time (JIT)** temporary privilege elevation
- Separation of regular and administrator accounts
- Strong authentication (**MFA**) for privileged access
- **Central password vault** (no account sharing)
- **Logging, monitoring, and session recording**

---
layout: default
---

# 8.2 Common Problems

- Regular users have **local administrator rights**
- Administrators log in directly on endpoints (locally)
- Anyone who asks gets what they want — no approval process
- Services run under a **user account** instead of a dedicated service account
