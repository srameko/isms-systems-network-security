---
layout: section
subtitle: ISO 27001 — Control 8.22
---

# Segregation of Networks

---
layout: default
---

# 8.22 Segregation of Networks

Ensures the network is **not one flat entity**, but a managed system of security zones that prevent the spread of attacks and reduce incident impact.

- Controlled division of the network into zones/segments
- Each zone has:
  - A different **trust level**
  - Different **communication rules**
- Goal: **limit lateral movement** and contain blast radius

---
layout: default
---

# 8.22 Why Segmentation?

<div class="icon-grid cols-2">
  <div class="icon-card">
    <div class="icon">❌</div>
    <div class="label"><strong>Without segmentation</strong><br/>Compromising one device can threaten the entire network</div>
  </div>
  <div class="icon-card">
    <div class="icon">✅</div>
    <div class="label"><strong>With segmentation</strong><br/>Attacker has a limited scope of action · Logical containment</div>
  </div>
</div>

**Protects against:**
- Lateral movement
- Internal threats

---
layout: default
---

# 8.22 Typical Segments

| Zone | Purpose |
|------|---------|
| **User network** | Workstations |
| **Server zone** | Internal services |
| **Management network** | Infrastructure administration |
| **VPN** | External access |
| **DMZ** | Public-facing services |
| **Guest (WiFi)** | Visitor access |
| **OT / ICS / IoT** | Industrial / production systems |

---
layout: default
---

# 8.22 Technical Controls

- **VLAN and routing**
- **Firewall types:**
  - Application (externally accessible services)
  - Perimeter (hides the whole network from outside)
  - Host-based (every device must have firewall enabled)
  - Global (cloud)
- **ACL** (Access Control Lists)
- **Microsegmentation** — virtualisation/cloud, down to NIC level

---
layout: default
---

# 8.22 Basic Rules

<div class="callout">
<strong>Default Deny</strong> — what is not explicitly allowed is forbidden
</div>

Allow only:
- Ports/services **strictly necessary** for operation
- **Specific sources and destinations**

**Regular rule review** — dead rules accumulate fast

---
layout: default
---

# 8.22 Common Problems

<div class="callout warning">
Flat networks are still extremely common — even in organisations that "have a firewall"
</div>

- No segmentation at all
- **Default allow** policies
- Missing or misconfigured firewalls
- Admin relies on a central firewall — but cloud workloads may not be behind it
- No guest network
- Servers and clients in the same subnet
- **No MFA for remote access** (VPN / RDP / SSH)

---
layout: center
---

# 🛠️ Group Exercise — 20 min

<div class="callout">
Imagine our fictional organisation: a bakery.
</div>

**Breakout Rooms — discuss:**

1. Describe the individual network segments (DMZ, WiFi, OT…)
2. Who can communicate with whom? And why?
3. What additional security controls could be used (FW, WAF, Proxy, IDS…) and where?

*(Network diagram on the next slide)*

---
layout: center
---

# 🏗️ Task: Network Security Architecture

**Breakout Rooms**

Design the network security architecture for the bakery organisation.
