---
layout: section
subtitle: ISO 27001 — Control 8.32
---

# Change Management

---
layout: default
---

# 8.32 Motivation

Every change to systems, infrastructure, and applications should be **planned, assessed, tested, approved, and documented** to prevent unintentional outages or security weaknesses.

- Partial exceptions exist (e.g. emergency patches)
- Eliminates **false positives** — security team knows what's happening at all times

---
layout: default
---

# 8.32 Change Management Process

A documented change management procedure exists, covering systems, applications, and infrastructure.

Changes are **classified** (routine, emergency) with appropriate workflow per type.

All non-trivial changes go through:

1. 📋 Planning
2. ⚠️ Risk assessment
3. ✅ Approval
4. 🧪 Testing
5. 🚀 Controlled deployment

---
layout: default
---

# 8.32 Changes in Practice

- Production changes **tested in a separate environment** first
- Security impact explicitly assessed for relevant changes (including security testing)
- Emergency changes are still:
  - Recorded
  - Authorised (even if via an expedited process)
  - Reviewed afterwards

**Change records must contain:**
> What was changed · Why · Who made the change · When and where · Outcome (including rollback if used)

---
layout: default
---

# 8.32 Workflow and Roles

<div class="icon-grid cols-2">
  <div class="icon-card">
    <div class="icon">✍️</div>
    <div class="label"><strong>Separation of duties</strong><br/>Approver ≠ Implementer — especially for critical systems</div>
  </div>
  <div class="icon-card">
    <div class="icon">📊</div>
    <div class="label"><strong>Metrics-driven improvement</strong><br/>Change success rate · incidents caused by changes · MTTR</div>
  </div>
</div>

Patch management follows the **same change process**, scaled to risk level.

---
layout: default
---

# 8.32 Metrics

| Metric | What it reveals |
|--------|----------------|
| Standard vs emergency change ratio | Process maturity |
| Volume by cadence (monthly/quarterly/yearly) | Planning effectiveness |
| Failed changes | Process quality and testing coverage |

---
layout: default
---

# 8.32 Common Problems

<div class="callout warning">
Shadow IT and untested changes are the biggest risks
</div>

- No testing before deployment
- Missing change documentation / evidence
- Missing or inadequate backups
- Ignoring updates and patches
- **Overly rigid process** — people work around it (Shadow IT)
- Shadow IT altogether
