---
layout: section
subtitle: ISO 27001 — Opatření 8.22
---

# Segmentace sítí

---
layout: default
---

# 8.22 Segmentace sítí

Zajišťuje, že síť **není jedním plochým celkem**, ale řízeným systémem bezpečnostních zón, které brání šíření útoků a snižují dopad incidentů.

- Řízené rozdělení sítě do zón/segmentů
- Každá zóna má:
  - Jinou **úroveň důvěry**
  - Jiná **pravidla komunikace**
- Cíl: **omezit laterální pohyb** a rozsah dopadu

---
layout: default
---

# 8.22 Proč segmentace?

<div class="icon-grid cols-2">
  <div class="icon-card">
    <div class="icon">❌</div>
    <div class="label"><strong>Bez segmentace</strong><br/>Kompromitace jednoho zařízení může ohrozit celou síť</div>
  </div>
  <div class="icon-card">
    <div class="icon">✅</div>
    <div class="label"><strong>Se segmentací</strong><br/>Útočník má omezený prostor pro pohyb · Logické omezení dopadu</div>
  </div>
</div>

**Ochrana proti:**
- Laterálnímu pohybu
- Interním hrozbám

---
layout: default
---

# 8.22 Typické segmenty

| Zóna | Účel |
|------|------|
| **Uživatelská síť** | Pracovní stanice |
| **Serverová zóna** | Interní služby |
| **Správcovská síť** | Správa infrastruktury |
| **VPN** | Vzdálený přístup |
| **DMZ** | Veřejně dostupné služby |
| **Host (WiFi)** | Přístup pro návštěvníky |
| **OT / ICS / IoT** | Průmyslové / výrobní systémy |

---
layout: default
---

# 8.22 Technická opatření

- **VLAN a směrování**
- **Typy firewallů:**
  - Aplikační (veřejně dostupné služby)
  - Perimetrální (skrývá celou síť před vnějškem)
  - Hostitelský (každé zařízení musí mít zapnutý firewall)
  - Globální (cloud)
- **ACL** (Access Control Lists)
- **Mikrosegmentace** — virtualizace/cloud, až na úroveň NIC

---
layout: default
---

# 8.22 Základní pravidla

<div class="callout">
<strong>Výchozí zamítnutí (Default Deny)</strong> — co není explicitně povoleno, je zakázáno
</div>

Povolujte pouze:
- Porty/služby **nezbytně nutné** pro provoz
- **Konkrétní zdroje a cíle**

**Pravidelná revize pravidel** — neaktuální pravidla se rychle hromadí

---
layout: default
---

# 8.22 Časté problémy

<div class="callout warning">
Ploché sítě jsou stále velmi běžné — i v organizacích, které „mají firewall"
</div>

- Žádná segmentace vůbec
- Zásady **výchozího povolení**
- Chybějící nebo chybně nakonfigurované firewally
- Správce spoléhá na centrální firewall — cloudové zátěže ale nemusí být za ním
- Žádná hostovská síť
- Servery a klienti ve stejné podsíti
- **Žádné MFA pro vzdálený přístup** (VPN / RDP / SSH)

---
layout: center
---

# 🛠️ Skupinové cvičení — 20 min

<div class="callout">
Představte si naši fiktivní organizaci: pekárnu.
</div>

**Breakout Rooms — diskutujte:**

1. Popište jednotlivé síťové segmenty (DMZ, WiFi, OT…)
2. Kdo může komunikovat s kým? A proč?
3. Jaká další bezpečnostní opatření by bylo možné použít (FW, WAF, Proxy, IDS…) a kde?

*(Síťový diagram na dalším slidu)*

---
layout: center
---

# 🏗️ Úkol: Architektura síťové bezpečnosti

**Breakout Rooms**

Navrhněte architekturu síťové bezpečnosti pro organizaci pekárny.
