---
layout: section
subtitle: ISO 27001 — Opatření 8.21
---

# Bezpečnost síťových služeb

---
layout: default
---

# 8.21 Motivace

Bezpečnost síťových služeb znamená zajistit, aby sítě, na nichž závisíte, byly **bezpečně specifikovány, poskytovány a průběžně monitorovány**.

Musíte se spoléhat na:
- Poskytovatele internetového připojení (ISP)
- Poskytovatele cloudu
- Poskytovatele řízené bezpečnosti (MSSP)
- Nebo jejich kombinaci

<div class="callout warning">
Pokud tyto síťové služby nejsou řádně zabezpečeny a spravovány, v podstatě předáváte veškeré své informace třetí straně.
</div>

---
layout: default
---

# 8.21 Dokumentace a SLA

- Organizace udržuje **aktuální inventář** všech klíčových síťových služeb (interních i externích) a jejich účelu
- Bezpečnostní požadavky (CIA, logování) jsou definovány **předem** pro síťové služby
- Smlouvy a SLA s poskytovateli obsahují:
  - Jasné bezpečnostní závazky
  - Definovaná SLA
  - Postupy pro reakci na incidenty
- Dokumentovaná **pravidla přístupu** (kdo má přístup k čemu, jak a za jakých podmínek)

---
layout: default
---

# 8.21 Bezpečnost a logování

**Implementovaná technická opatření:**

<div class="icon-grid">
  <div class="icon-card">
    <div class="icon">🔒</div>
    <div class="label">Šifrování</div>
  </div>
  <div class="icon-card">
    <div class="icon">🧱</div>
    <div class="label">Firewally</div>
  </div>
  <div class="icon-card">
    <div class="icon">🗂️</div>
    <div class="label">Síťová segmentace</div>
  </div>
  <div class="icon-card">
    <div class="icon">⚙️</div>
    <div class="label">Bezpečné konfigurace</div>
  </div>
  <div class="icon-card">
    <div class="icon">🔑</div>
    <div class="label">MFA</div>
  </div>
</div>

Využívání a správa síťových služeb musí být **zaznamenávány a monitorovány** s upozorněními na podezřelou aktivitu.

---
layout: default
---

# 8.21 Testování, BCP & DR a školení

- Síťové služby podléhají **bezpečnostnímu testování** a pravidelným revizím (včetně revizí po změnách)
- Odolnost (redundance, failover) je navržena a propojena s **BCP/DR**
- Správci a relevantní zaměstnanci jsou školeni v **bezpečné správě** a používání síťových služeb

---
layout: default
---

# 8.21 Metriky

| Oblast | Metrika |
|--------|---------|
| Hosting | Dostupnost webové prezentace |
| Uplink | Konektivita ISP |
| Datové centrum | Externí DC a jeho služby |
| Služby | Dostupnost služeb (příchozí i odchozí) |
| Logování | Objem shromážděných logů |
| Vzory provozu | Periodicita (víkendy, svátky, Black Friday…) |

---
layout: default
---

# 8.21 Časté problémy

<div class="callout warning">
Chybějící redundance konektivity/hostingu je nejčastější bod selhání
</div>

- Žádná redundance pro konektivitu / hosting / VPS / datové centrum
- **Nevyužité možnosti ISP**: ochrana proti DDoS, RTBH
- Nedostatečná smluvní specifikace s poskytovateli
  - Chybějící definice služeb
  - Slabá nebo chybějící SLA

---
layout: center
---

# ☕ Přestávka
