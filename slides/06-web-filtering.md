---
layout: section
subtitle: ISO 27001 — Opatření 8.23
---

# Webové filtrování

---
layout: default
---

# 8.23 Motivace

<div class="callout warning">
Webový prohlížeč je jedním z nejčastějších vektorů útoku — uživatelé klikají rychleji, než bezpečnostní tým stačí reagovat.
</div>

**Webové filtrování:**
- Snižuje riziko lidské chyby
- Blokuje útoky **dříve, než se projeví**

**Napětí mezi bezpečností a soukromím:**
- Bezpečnostní tým vidí všechny URL, které uživatel navštěvuje
- Stejná výzva jako u monitorování e-mailů

---
layout: default
---

# 8.23 Webové filtrování

<div class="callout">
Webové filtrování neomezuje uživatele — chrání organizaci před nejčastějšími útoky z internetu. Je to jedno z nejefektivnějších preventivních opatření.
</div>

**Rozsah:**
- Řídí a omezuje přístup na webové stránky
- Chrání před malwarem, phishingem, škodlivým a nevhodným obsahem

---
layout: default
---

# 8.23 Běžné kategorie filtrů

<div class="icon-grid">
  <div class="icon-card">
    <div class="icon">☠️</div>
    <div class="label">Škodlivé weby (hostující škodlivý obsah)</div>
  </div>
  <div class="icon-card">
    <div class="icon">🎣</div>
    <div class="label">Phishingové weby</div>
  </div>
  <div class="icon-card">
    <div class="icon">🔞</div>
    <div class="label">Nežádoucí kategorie (zbraně, drogy, pornografie)</div>
  </div>
  <div class="icon-card">
    <div class="icon">🏴‍☠️</div>
    <div class="label">Pirátský obsah</div>
  </div>
  <div class="icon-card">
    <div class="icon">🆕</div>
    <div class="label">Nově registrované / neznámé domény (bez historie)</div>
  </div>
</div>

---
layout: default
---

# 8.23 Související opatření

Webové filtrování se váže na:

| Opatření | Popis |
|----------|-------|
| **8.7** | Ochrana před malwarem |
| **8.22** | Segmentace sítí |
| **6.3** | Osvěta a školení |
| **8.16** | Monitorování aktivit |

Webové filtrování je **technické i preventivní** opatření.
Může být součástí firewallového řešení nebo **samostatné služby**.

---
layout: default
---

# 8.23 Metriky

- Procento celkového provozu, který je **blokován**
- Které **kategorie** se objevují nejčastěji
- Které konkrétní **weby** jsou nejnavštěvovanější (dnes zejména AI — riziko úniku dat)
- Kategorie, které se objevují **velmi zřídka**
- Kolik URL je nutné **ručně přidat** (typicky phishing nebo nové škodlivé weby)

---
layout: default
---

# 8.23 Časté problémy

<div class="callout warning">
Filtrovat pouze známé služby? Nové (podezřelé) ještě nejsou v seznamech — riziko úniku dat.
</div>

- **Žádné filtrování vůbec** — kdokoli může jít kamkoli
- Filtr pokrývá pouze známé služby (např. pouze známé AI nástroje)
  - Nové (pochybné) ještě nejsou ve filtrovacích seznamech
- Chybějící **granularita:**
  - HR potřebuje přístup na web XY
  - Finance potřebuje přístup na web AB, ale ne XY
  - Řadoví zaměstnanci by neměli mít přístup ani na AB, ani na XY

---
layout: center
---

# ☕ Přestávka
