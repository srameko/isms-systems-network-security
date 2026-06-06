---
layout: section
subtitle: ISO 27001 — Control 8.21
---

# Security of Network Services

---
layout: default
---

# 8.21 Motivation

Network service security means ensuring that networks you depend on are **securely specified, delivered, and continuously monitored**.

You must rely on:
- Internet Service Provider (ISP)
- Cloud provider
- Managed Security Service Provider
- Or a combination

<div class="callout warning">
If these network services are not properly secured and managed, you are essentially handing all your information to a third party.
</div>

---
layout: default
---

# 8.21 Documentation and SLAs

- The organisation maintains an **up-to-date inventory** of all key network services (internal and external) and their purpose
- Security requirements (CIA, logging) are defined **upfront** for network services
- Contracts and SLAs with providers contain:
  - Clear security obligations
  - Defined SLAs
  - Incident response procedures
- Documented **access rules** (who has access to what, how, and under what conditions)

---
layout: default
---

# 8.21 Security and Logging

**Technical controls implemented:**

<div class="icon-grid">
  <div class="icon-card">
    <div class="icon">🔒</div>
    <div class="label">Encryption</div>
  </div>
  <div class="icon-card">
    <div class="icon">🧱</div>
    <div class="label">Firewalls</div>
  </div>
  <div class="icon-card">
    <div class="icon">🗂️</div>
    <div class="label">Network Segmentation</div>
  </div>
  <div class="icon-card">
    <div class="icon">⚙️</div>
    <div class="label">Secure Configurations</div>
  </div>
  <div class="icon-card">
    <div class="icon">🔑</div>
    <div class="label">MFA</div>
  </div>
</div>

Usage and management of network services must be **logged and monitored** with alerts on suspicious activity.

---
layout: default
---

# 8.21 Testing, BCP & DR, and Training

- Network services subject to **security testing** and regular reviews (including post-change reviews)
- Resilience (redundancy, failover) designed and linked with **BCP/DR**
- Administrators and relevant staff trained in **secure management** and use of network services

---
layout: default
---

# 8.21 Metrics

| Area | Metric |
|------|--------|
| Hosting | Web presence availability |
| Uplink | ISP connectivity |
| Datacenter | External DC and its services |
| Services | Availability of services (inbound and outbound) |
| Logging | Volume of logs collected |
| Traffic patterns | Periodicity (weekends, holidays, Black Friday…) |

---
layout: default
---

# 8.21 Common Problems

<div class="callout warning">
Missing connectivity/hosting redundancy is the most common failure point
</div>

- No redundancy for connectivity / hosting / VPS / datacenter
- **Unused ISP capabilities**: DDoS protection, RTBH
- Insufficient contract specification with providers
  - Missing service definitions
  - Weak or absent SLAs

---
layout: center
---

# ☕ Break
