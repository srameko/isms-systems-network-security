---
layout: section
subtitle: ISO 27001 — Opatření 8.2
---

# PAM / PIM — Správa privilegovaného přístupu

---
layout: default
---

# 8.2 Privilegovaná přístupová práva / správa

Privilegované účty představují **nejvyšší riziko** v případě kompromitace.

Opatření 8.2 zajišťuje, že jsou přísně spravovány, monitorovány a používány pouze tehdy, je-li to nezbytné.

**V rozsahu:**
- Administrátorské a systémové účty
- Účty umožňující:
  - Změny konfigurace
  - Instalaci softwaru
  - Správu uživatelů
  - Přístup k citlivým datům

---
layout: default
---

# 8.2 Privilegovaná přístupová práva

Cíl: zajistit, aby privilegovaná přístupová práva (admin, root, enterprise admin) byla udělována, používána a spravována **řízeným způsobem** — snižujícím riziko zneužití nebo kompromitace.

<div class="callout">
V praxi se typicky používá komerční software PAM: <strong>CyberArk, BeyondTrust</strong> a podobná řešení.
</div>

---
layout: default
---

# 8.2 PAM — Základní principy

**Nejnižší oprávnění (Least Privilege)**

- Privilegovaný přístup pouze pro **oprávněné osoby**
- Pouze po **minimálně nutnou dobu** (na vyžádání / časově omezený)

**Oddělení účtů**

- Běžné uživatelské účty
- Administrátorské účty
- V praxi: více úrovní oprávnění (R, RW…)

---
layout: default
---

# 8.2 PAM — Klíčové požadavky

<div class="icon-grid">
  <div class="icon-card">
    <div class="icon">📋</div>
    <div class="label">Formální proces pro schvalování, změny a odvolání</div>
  </div>
  <div class="icon-card">
    <div class="icon">📅</div>
    <div class="label">Evidence a pravidelná revize přístupů (typicky roční)</div>
  </div>
  <div class="icon-card">
    <div class="icon">🔑</div>
    <div class="label">MFA (Passkeys, Push notifikace…)</div>
  </div>
  <div class="icon-card">
    <div class="icon">📝</div>
    <div class="label">Logování a monitoring veškeré privilegované aktivity</div>
  </div>
</div>

---
layout: default
---

# 8.2 PAM — Role a odpovědnosti

| Role | Odpovědnost |
|------|-------------|
| **Vedení** | Schvaluje politiky a výjimky |
| **Bezpečnost** | Kontroluje a audituje privilegované účty |
| **IAM** | Spravuje privilegované účty |
| **Uživatelé** | Odpovídají za bezpečné používání svého přístupu |

---
layout: default
---

# 8.2 Co nedělat

**Typické příklady**

<div class="callout warning">
Zapomenuté nebo nezaznamenané účty s administrátorským přístupem (včetně Shadow IT)
</div>

- Žádné logování ani monitoring
- Žádné MFA
- Sdílení přihlašovacích údajů pro generické účty jako `admin42@org.cz`
- Slabá hesla

**Výsledná rizika**

- Ztráta dat
- Narušení integrity
- Narušení dostupnosti

---
layout: default
---

# PAM — Shrnutí

**Správa privilegovaného přístupu** zahrnuje:

- Správu a zabezpečení privilegovaných účtů (admin, root, servisní účty)
- Omezení přístupu dle principu **nejnižších oprávnění**
- **Just-In-Time (JIT)** dočasné zvýšení oprávnění
- Oddělení běžných a administrátorských účtů
- Silná autentizace (**MFA**) pro privilegovaný přístup
- **Centrální trezor hesel** (žádné sdílení účtů)
- **Logování, monitoring a nahrávání relací**

---
layout: default
---

# 8.2 Časté problémy

- Běžní uživatelé mají **práva lokálního administrátora**
- Administrátoři se přihlašují přímo na koncových stanicích (lokálně)
- Kdokoli, kdo požádá, dostane co chce — žádný schvalovací proces
- Služby běží pod **uživatelským účtem** místo dedikovaného servisního účtu
