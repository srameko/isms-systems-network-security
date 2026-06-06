---
layout: section
subtitle: ISO 27001 — Opatření 8.20
---

# Bezpečnost sítí

---
layout: default
---

# 8.20 Bezpečnost sítí

**Existuje dokumentovaný standard síťové bezpečnosti**, který zahrnuje:

- Definované **síťové zóny**
- Povolené **datové toky**

Standard musí být:
- Srozumitelný
- Aktuální
- Skutečně používán v praxi

---
layout: default
---

# 8.20 Hardening zařízení

Síťová zařízení musí být:

| Požadavek | Příklady |
|-----------|---------|
| **Hardenovaná** | Minimální služby, bezpečné výchozí nastavení |
| **Aktualizovaná** | Pravidelné cykly záplatování |
| **Spravovaná** | Centralizovaná správa konfigurace |

Platí pro **vše se správcovským rozhraním**:
Firewally · Routery · Switche · VPN · Tiskárny · Přístupové body

---
layout: default
---

# 8.20 Přístup k síti

- Síť je rozdělena do **bezpečnostních zón**
  - Host · DMZ · ICS/IoT/SCADA
- Kritické systémy jsou:
  - Izolovány
  - Chráněny přísnějšími pravidly
- **Autentizace na úrovni zařízení** pro přístup k síti

---
layout: default
---

# 8.20 Vzdálený a bezdrátový přístup

**Vzdálený přístup (VPN)**
- Vícefaktorová autentizace (MFA) a další bezpečnostní kroky
- Šifrování

**Wi-Fi**
- Oddělené sítě pro zaměstnance a hosty
- Ověřování přístupu

---
layout: default
---

# 8.20 Logování a monitoring

Klíčové síťové události musí být:
- **Zaznamenávány**
- **Monitorovány**

Organizace musí být schopna:
- Detekovat podezřelý provoz
- Vyšetřovat incidenty

---
layout: default
---

# 8.20 Cloud vs. On-Premise

<div class="icon-grid cols-2">
  <div class="icon-card">
    <div class="icon">☁️</div>
    <div class="label"><strong>Cloud</strong><br/>Stejné bezpečnostní principy platí — cloud není výjimkou z bezpečnosti</div>
  </div>
  <div class="icon-card">
    <div class="icon">🏢</div>
    <div class="label"><strong>On-Premise</strong><br/>Opatření jsou definována a dokumentována, pravidelně revidována</div>
  </div>
</div>

<div class="callout warning">
Cloud není výjimkou z bezpečnostních požadavků.
</div>

---
layout: default
---

# 8.20 Správa změn

Síťové změny musí procházet:
- **Procesem správy změn**
- Schvalovacím postupem
- Pravidla jsou **pravidelně revidována**

---
layout: default
---

# 8.20 Audit

Organizace musí být schopna prokázat:

- Konfigurace
- Síťové diagramy
- Logy
- Záznamy o změnách

Bezpečnost musí být **prokazatelná a udržitelná**.

---
layout: default
---

# 8.20 Metriky

| Metrika | Popis |
|---------|-------|
| Stav zařízení | Kolik je aktuálních |
| Přihlášení | Úspěšná vs. neúspěšná autentizace |
| Ztráta paketů | Indikátor zdraví sítě |
| Připojená zařízení | Počet kabelových / bezdrátových / hostovských |

---
layout: default
---

# 8.20 Časté problémy

<div class="callout warning">
Cloud je často ponechán bez správy — výchozí nastavení ponechána, nikdo nemonitoruje
</div>

- Nikdo nemonitoruje síťový provoz
- Správcovská rozhraní jsou dostupná z internetu
- Slabá nebo chybějící autentizace
- Nelze dohledat, které zařízení způsobilo incident
