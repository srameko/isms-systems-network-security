---
layout: section
subtitle: ISO 27001 — Opatření 8.32
---

# Správa změn

---
layout: default
---

# 8.32 Motivace

Každá změna systémů, infrastruktury a aplikací by měla být **plánovaná, posouzená, otestovaná, schválená a zdokumentovaná**, aby se předešlo neúmyslným výpadkům nebo bezpečnostním slabinám.

- Částečné výjimky existují (např. havarijní záplaty)
- Eliminuje **falešné poplachy** — bezpečnostní tým ví, co se děje

---
layout: default
---

# 8.32 Proces správy změn

Existuje dokumentovaný postup správy změn pokrývající systémy, aplikace a infrastrukturu.

Změny jsou **klasifikovány** (rutinní, havarijní) s příslušným pracovním postupem dle typu.

Všechny netriviální změny procházejí:

1. 📋 Plánování
2. ⚠️ Posouzení rizik
3. ✅ Schválení
4. 🧪 Testování
5. 🚀 Řízené nasazení

---
layout: default
---

# 8.32 Změny v praxi

- Produkční změny **nejdříve testovány v oddělené prostředí**
- Bezpečnostní dopad je explicitně posouzen pro relevantní změny (včetně bezpečnostního testování)
- Havarijní změny jsou vždy:
  - Zaznamenány
  - Autorizovány (i když zrychleným procesem)
  - Zpětně přezkoumány

**Záznamy o změnách musí obsahovat:**
> Co bylo změněno · Proč · Kdo změnu provedl · Kdy a kde · Výsledek (včetně rollbacku, pokud byl použit)

---
layout: default
---

# 8.32 Pracovní postup a role

<div class="icon-grid cols-2">
  <div class="icon-card">
    <div class="icon">✍️</div>
    <div class="label"><strong>Oddělení povinností</strong><br/>Schvalovatel ≠ Realizátor — zejména pro kritické systémy</div>
  </div>
  <div class="icon-card">
    <div class="icon">📊</div>
    <div class="label"><strong>Zlepšování na základě metrik</strong><br/>Míra úspěšnosti změn · incidenty způsobené změnami · MTTR</div>
  </div>
</div>

Správa záplat se řídí **stejným procesem správy změn**, upraveným podle úrovně rizika.

---
layout: default
---

# 8.32 Metriky

| Metrika | Co odhaluje |
|---------|-------------|
| Poměr standardních a havarijních změn | Vyspělost procesu |
| Objem dle kadence (měsíčně/čtvrtletně/ročně) | Efektivita plánování |
| Neúspěšné změny | Kvalita procesu a pokrytí testováním |

---
layout: default
---

# 8.32 Časté problémy

<div class="callout warning">
Shadow IT a netestované změny jsou největšími riziky
</div>

- Žádné testování před nasazením
- Chybějící dokumentace / evidence o změnách
- Chybějící nebo nedostatečné zálohy
- Ignorování aktualizací a záplat
- **Příliš rigidní proces** — lidé ho obcházejí (Shadow IT)
- Shadow IT celkově
