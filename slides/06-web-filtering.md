---
layout: section
subtitle: ISO 27001 — Control 8.23
---

# Web Filtering

---
layout: default
---

# 8.23 Motivation

<div class="callout warning">
The web browser is one of the most common attack vectors — users click faster than the security team can react.
</div>

**Web filtering:**
- Reduces the risk of human error
- Blocks attacks **before they land**

**Security vs. Privacy tension:**
- The security team can see all URLs a user visits
- Same challenge as with email monitoring

---
layout: default
---

# 8.23 Web Filtering

<div class="callout">
Web filtering doesn't restrict users — it protects the organisation from the most common internet-based attacks. It's one of the most effective preventive controls.
</div>

**Scope:**
- Governs and limits access to websites
- Protects against malware, phishing, malicious and inappropriate content

---
layout: default
---

# 8.23 Common Filter Categories

<div class="icon-grid">
  <div class="icon-card">
    <div class="icon">☠️</div>
    <div class="label">Malicious sites (hosting harmful content)</div>
  </div>
  <div class="icon-card">
    <div class="icon">🎣</div>
    <div class="label">Phishing sites</div>
  </div>
  <div class="icon-card">
    <div class="icon">🔞</div>
    <div class="label">Undesirable categories (weapons, drugs, pornography)</div>
  </div>
  <div class="icon-card">
    <div class="icon">🏴‍☠️</div>
    <div class="label">Pirated content</div>
  </div>
  <div class="icon-card">
    <div class="icon">🆕</div>
    <div class="label">Newly registered / unknown domains (no history)</div>
  </div>
</div>

---
layout: default
---

# 8.23 Related Controls

Web filtering connects to:

| Control | Description |
|---------|-------------|
| **8.7** | Malware protection |
| **8.22** | Segregation of networks |
| **6.3** | Awareness & training |
| **8.16** | Monitoring activities |

Web filtering is both a **technical and preventive** control.
It can be part of a firewall solution or a **dedicated service**.

---
layout: default
---

# 8.23 Metrics

- Percentage of total traffic that is **blocked**
- Which **categories** appear most frequently
- Which specific **sites** are most accessed (today especially AI — data leakage concerns)
- Categories that appear **very rarely**
- How many URLs must be **manually added** (typically phishing or new malicious sites)

---
layout: default
---

# 8.23 Common Problems

<div class="callout warning">
Filter only on known services? New (suspicious) ones won't be in the lists yet — data leakage risk.
</div>

- **No filtering at all** — anyone can go anywhere
- Filter covers only known services (e.g. only known AI tools)
  - New ones (questionable) not yet in filter lists
- Missing **granularity:**
  - HR needs access to site XY
  - Finance needs access to site AB but not XY
  - Regular employees should have access to neither AB nor XY

---
layout: center
---

# ☕ Break
