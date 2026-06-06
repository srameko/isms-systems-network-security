---
layout: section
subtitle: ISO 27001 — Opatření 8.31
---

# Oddělení vývojového, testovacího a produkčního prostředí

---
layout: default
---

# 8.31 Motivace

<div class="callout">
Klíčové opatření pro provozní stabilitu a bezpečnost — zajišťuje, aby chyby ve vývoji a testech neohrožovaly produkci.
</div>

- Ochrana produkčních dat a systémů
- Snížení rizika chyb a incidentů
- **Klenoty koruny** (produkční data a systémy) zůstávají chráněny

---
layout: default
---

# 8.31 Proč na tom záleží

<div class="icon-grid cols-2">
  <div class="icon-card">
    <div class="icon">❌</div>
    <div class="label"><strong>Bez oddělení</strong><br/>Testovací kód v produkci · Neoprávněné změny · Únik nebo zneužití dat</div>
  </div>
  <div class="icon-card">
    <div class="icon">✅</div>
    <div class="label"><strong>S oddělením</strong><br/>Řízené změny · Nižší riziko výpadků · Jasná odpovědnost</div>
  </div>
</div>

---
layout: default
---

# 8.31 Typická prostředí

| Prostředí | Účel | Data |
|-----------|------|------|
| **Vývoj** | Psaní a úpravy kódu | Anonymizovaná/maskovaná |
| **Test / QA** | Funkční a bezpečnostní testování, ověřování změn | Anonymizovaná/maskovaná |
| **Produkce** | Živý provoz, skuteční uživatelé | Skutečná data |

Každé prostředí má **jiná pravidla a oprávnění**.

---
layout: default
---

# 8.31 Jak to funguje

**Dedikované pro každé prostředí:**
- Systémy / servery
- Přístupová práva
- Sítě (viz 8.22)

**Žádný přímý vývoj ani testování v produkci**

**Přesun do produkce:**
- Pouze přes schválený proces (**Správa změn**)
- Minimální počet osob s přístupem k PROD (**PAM**)

---
layout: default
---

# 8.31 Práce s daty

<div class="callout warning">
Produkční data nesmí být nikdy použita ve vývojovém ani testovacím prostředí.
</div>

**Vývojová / testovací prostředí používají:**
- Anonymizovaná data
- Maskovaná data
- Syntetická data

**Proč na tom záleží:**
- Ochrana osobních a citlivých dat
- Soulad s **GDPR** a **ISO 27001**

---
layout: default
---

# 8.31 Časté problémy

<div class="callout warning">
Tajné informace (tokeny, API klíče…) ve veřejných repozitářích (GitHub/GitLab/Bitbucket) jsou kritickým a častým incidentem
</div>

- Dev/testovací server dostupný z internetu
- Špatná bezpečnostní konfigurace (slabé nebo žádné heslo, chybějící záplaty)
- **Tajné informace ve veřejných repozitářích** — tokeny, API klíče, přihlašovací údaje
- **Produkční data tam, kde by neměla být**
