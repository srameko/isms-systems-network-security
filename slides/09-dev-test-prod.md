---
layout: section
subtitle: ISO 27001 — Control 8.31
---

# Separation of Development, Test, and Production

---
layout: default
---

# 8.31 Motivation

<div class="callout">
Key control for operational stability and security — ensures that errors in development and test do not threaten production.
</div>

- Protection of production data and systems
- Reduction of risk of errors and incidents
- **Crown jewels** (production data and systems) remain protected

---
layout: default
---

# 8.31 Why It Matters

<div class="icon-grid cols-2">
  <div class="icon-card">
    <div class="icon">❌</div>
    <div class="label"><strong>Without separation</strong><br/>Test code in production · Unauthorised changes · Data leakage or misuse</div>
  </div>
  <div class="icon-card">
    <div class="icon">✅</div>
    <div class="label"><strong>With separation</strong><br/>Controlled changes · Lower risk of outages · Clear accountability</div>
  </div>
</div>

---
layout: default
---

# 8.31 Typical Environments

| Environment | Purpose | Data |
|-------------|---------|------|
| **Development** | Code writing and modifications | Anonymised/masked |
| **Test / QA** | Functional and security testing, change verification | Anonymised/masked |
| **Production** | Live operation, real users | Real data |

Each environment has **different rules and permissions**.

---
layout: default
---

# 8.31 How It Works

**Dedicated per environment:**
- Systems / servers
- Access rights
- Networks (see 8.22)

**No direct development or testing in production**

**Moving to production:**
- Only through an approved process (**Change Management**)
- Minimum number of people with PROD access (**PAM**)

---
layout: default
---

# 8.31 Data Handling

<div class="callout warning">
Production data must never be used in development or test environments.
</div>

**Development / Test environments use:**
- Anonymised data
- Masked data
- Synthetic data

**Why it matters:**
- Protection of personal and sensitive data
- Compliance with **GDPR** and **ISO 27001**

---
layout: default
---

# 8.31 Common Problems

<div class="callout warning">
Secrets (tokens, API keys…) appearing in public repositories (GitHub/GitLab/Bitbucket) is a critical and frequent incident
</div>

- Dev/test server accessible from the internet
- Poor security posture (weak or no password, missing patches)
- **Secrets in public repos** — tokens, API keys, credentials
- **Production data where it shouldn't be**
