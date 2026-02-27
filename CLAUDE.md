# CLAUDE.md — Přijímací zkoušky na gymnázium (CERMAT)

Tento soubor říká Claudovi, jak se chovat při práci s přijímacími testy v tomto workspace.

---

## Nastavení pro nového studenta

**Při prvním spuštění** (pokud sekce „Kontext studenta" níže není vyplněna) proveď celý onboarding pomocí nástroje `AskUserQuestion`. Ptej se ve 4 kolech — každé kolo jsou 2–4 otázky najednou jako interaktivní popup s možnostmi výběru. Nezahazuj odpovědi — po všech 4 kolech doplň sekci „Kontext studenta" níže a ulož soubor.

Začni krátkým uvítáním (1–2 věty), pak spusť Kolo 1.

---

### Kolo 1 — Základní info (AskUserQuestion, 2 otázky)

**Otázka 1: „Jak se jmenuješ?"**
- Odpověď je volný text — použij možnost „Other" nebo nech studenta napsat do chatu.

**Otázka 2: „Na jak konkurenční školu se hlásíš?"**
Možnosti:
- „Velmi konkurenční (Praha centrum, Brno centrum, elitní školy)" — cílové skóre 85+/100
- „Středně konkurenční (krajské město, dobrá škola)" — cílové skóre 70–85/100
- „Méně konkurenční (menší město, regionální gymnázium)" — cílové skóre 60–70/100
- „Ještě nevím / více škol" — nastavíme cíl po prvních testech

---

### Kolo 2 — Aktuální úroveň (AskUserQuestion, 3 otázky)

**Otázka 1: „Jak bys ohodnotil/a svoji matematiku?"**
Možnosti:
- „1–4: Matematika mi moc nejde, hodně věcí mi chybí"
- „5–6: Průměr — základy umím, ale chybuji v detailech"
- „7–8: Dobré — chápu látku, chyby dělám spíš z nepozornosti"
- „9–10: Matematika mi jde velmi dobře"

**Otázka 2: „Jak bys ohodnotil/a svoji češtinu?"**
Možnosti:
- „1–4: Čeština mi dělá velké problémy (gramatika, pravopis, texty)"
- „5–6: Průměr — texty zvládám, ale gramatika/syntax mi dělá problémy"
- „7–8: Docela dobře — chybuji hlavně ve složitějších jevech"
- „9–10: Čeština mi jde velmi dobře"

**Otázka 3: „Kde hlavně děláš chyby?"**
Možnosti:
- „Chybí mi látka — neznám postup nebo vzorec"
- „Dělám chyby z nepozornosti — postup znám, ale přepočítám se nebo špatně přečtu"
- „Obojí přibližně stejně"
- „Ještě nevím — tohle zjistíme z testů"

---

### Kolo 3 — Čas a přístup k materiálům (AskUserQuestion, 3 otázky)

**Otázka 1: „Kolik hodin týdně reálně můžeš věnovat přípravě?"**
Možnosti:
- „Méně než 2 hodiny — mám málo času"
- „2–5 hodin — standardní příprava"
- „5–10 hodin — intenzivní příprava"
- „Více než 10 hodin — chci se připravit opravdu důkladně"

**Otázka 2: „Jak se připravuješ?"**
Možnosti:
- „Sám/sama — bez doučování"
- „Mám soukromé doučování"
- „Chodím na přípravný kurz nebo kroužek"
- „Kombinuju více způsobů"

**Otázka 3: „Máš přístup k testům z minulých let?"**
Možnosti:
- „Ano — stahuju si je z webu CERMAT nebo Scio"
- „Ano — mám je z kurzu nebo od učitele"
- „Nemám — poraď mi, kde je sehnat"
- „Mám jen některé"

---

### Kolo 4 — Preference zpětné vazby (AskUserQuestion, 2 otázky)

**Otázka 1: „Jak chceš dostávat zpětnou vazbu po testech?"**
Možnosti:
- „Stručně — jen co jsem pokazil/a a co mám procvičit"
- „Podrobně — chci vysvětlení každé chyby krok po kroku"

**Otázka 2: „Jaký přístup ti víc vyhovuje?"**
Možnosti:
- „Motivační — oceňuju povzbuzení a pozitivní zpětnou vazbu"
- „Věcný — chci jen fakta, bez zbytečných komentářů"

---

### Po onboardingu

1. Shrň profil studenta v 2–3 větách (co umí, kolik má času, co od tebe čeká)
2. Nastav cílové skóre podle odpovědí (škola + sebehodnocení)
3. Doplň celou sekci „Kontext studenta" níže a ulož soubor
4. Navrhni první krok — konkrétně:
   - Pokud student má test: „Nahraj PDF zadání a fotky svých odpovědí — rovnou to analyzuji"
   - Pokud nemá: „Stáhni si test z cermat.cz — například MA_2024_9A — a vrať se"
---

## Struktura složek

```
Prijimaci zkousky/
├── CLAUDE.md                          ← tento soubor (instrukce pro Clauda)
├── README.md                          ← přehled pro studenta
├── Matematika/
│   ├── _Prehled.md                    ← celkový přehled výkonu v matematice
│   └── RRRR-MM-DD_<kod_testu>/        ← jeden subfolder = jeden test
│       ├── zadani.pdf                 ← PDF se zadáním
│       ├── vysledky_str1.jpg          ← foto/screenshot odpovědí (strany 1, 2, ...)
│       ├── vysledky_str2.jpg
│       ├── Analyza.md                 ← analýza tohoto testu
│       └── Studijni_plan.md           ← doporučený plán studia po tomto testu
└── Cesky jazyk/
    ├── _Prehled.md                    ← celkový přehled výkonu v češtině
    └── RRRR-MM-DD_<kod_testu>/
        ├── zadani.pdf
        ├── vysledky_str1.jpg
        ├── Analyza.md
        └── Studijni_plan.md
```

**Pojmenování testu:** `RRRR-MM-DD_<zkratka>` — příklady:
- `2026-03-15_MA_2025_9A` (matematika, rok 2025, verze 9A)
- `2026-03-15_CJL_2025_9B` (český jazyk, rok 2025, verze 9B)

---

## Postup při přijetí nového testu

### Krok 1 — Příjem souborů

- **Nahrané přímo do chatu:** zpracuj z `/sessions/.../mnt/uploads/`
- **Ve workspace:** hledej v `Matematika/` nebo `Cesky jazyk/`
- **Formát HEIC:** převeď: `convert soubor.heic soubor.jpg`

### Krok 2 — Vytvoření subfolderů

```bash
mkdir -p "Matematika/RRRR-MM-DD_<kod>/"
# nebo
mkdir -p "Cesky jazyk/RRRR-MM-DD_<kod>/"
```

Přesuň nebo zkopíruj:
- Zadání → `zadani.pdf`
- Fotky odpovědí → `vysledky_str1.jpg`, `vysledky_str2.jpg`, ...

### Krok 3 — Analýza

Přečti:
1. `zadani.pdf` — celé zadání a bodování
2. Klíč správných odpovědí (pokud ho student dodal) — jinak vyřeš úlohy sám
3. Všechny `vysledky_str*.jpg` — přečti odpovědi studenta

Porovnej každou odpověď s klíčem. Spočítej skóre. Zapiš analýzu do `Analyza.md` (viz šablona níže).

### Krok 4 — Uložení výsledků

1. Ulož `Analyza.md` do subfolderů testu
2. Aktualizuj `_Prehled.md` příslušného předmětu:
   - Přidej řádek do tabulky skóre (s odkazem na `Analyza.md`)
   - Aktualizuj sekce „Silné oblasti", „Slabé oblasti", „Trend"
3. Aktualizuj `README.md` — tabulku „Přehled testů"

---

## Šablona Analyza.md

### Pro matematiku

```markdown
# Analýza testu — <název testu>

**Datum vypracování:** DD. M. RRRR
**Verze testu:** <kód>
**Soubory:** zadani.pdf, vysledky_str1–N.jpg

---

## Výsledek: X / 50 bodů (Z %)

| Oblast | Max bodů | Získáno | % úspěšnosti |
|--------|----------|---------|--------------|
| Čísla a početní operace | ~10 b | | |
| Algebra (výrazy, rovnice) | ~10 b | | |
| Geometrie (rovinná + tělesa) | ~12 b | | |
| Slovní úlohy a kombinatorika | ~10 b | | |
| Statistika a pravděpodobnost | ~5 b | | |
| Konstrukce | ~3 b | | |
| **Celkem** | **50 b** | | |

---

## Chyby

### Chyba 1 — Úloha X: <stručný název>

**Správná odpověď:** ...
**Odpověď studenta:** ...
**Typ chyby:** [konceptuální / početní / chybný zápis / záměna vzorce / špatný převod textu / nepozornost]
**Rozbor:** ...
**Co procvičit:** ...

### Chyba 2 — ...

---

## Časová analýza (pokud jsou dostupné informace)

- Odhadovaný čas na test: X min z 70 min
- Úlohy přeskočené nebo nedokončené: ...

---

## Doporučení pro studium

Na základě chyb v tomto testu procvičit:
1. [Konkrétní téma + konkrétní typ úlohy — ne obecné „geometrie"]
2. ...
```

### Pro český jazyk

```markdown
# Analýza testu — <název testu>

**Datum vypracování:** DD. M. RRRR
**Verze testu:** <kód>
**Soubory:** zadani.pdf, vysledky_str1–N.jpg

---

## Výsledek: X / 50 bodů (Z %)

| Oblast | Max bodů | Získáno | % úspěšnosti |
|--------|----------|---------|--------------|
| Porozumění textu | ~20 b | | |
| Gramatika a pravopis | ~12 b | | |
| Syntax a stavba věty | ~10 b | | |
| Slovní zásoba a slohové prostředky | ~8 b | | |
| **Celkem** | **50 b** | | |

---

## Chyby

### Chyba 1 — Úloha X: <stručný název>

**Správná odpověď:** ...
**Odpověď studenta:** ...
**Typ chyby:** [neporozumění textu / gramatická chyba / pravopis / syntax / slovní zásoba / nesprávná interpretace otázky]
**Rozbor:** ...
**Co procvičit:** ...

### Chyba 2 — ...

---

## Doporučení pro studium

1. [Konkrétní téma — ne obecné „procvičit gramatiku", ale např. „shoda přísudku s podmětem u jmenných skupin"]
2. ...
```

---

## Pravidla analýzy

1. **Matematicky ověř každou odpověď** — nespoléhej jen na vizuální čtení obrázků.
2. **Klíč správných odpovědí:** Pokud ho student dodá, použij ho jako primární zdroj. Pokud ne, vyřeš úlohy sám a uveď to v analýze.
3. **Pojmenování chyb:** Vždy uveď typ chyby (viz šablona výše). Typ chyby určuje, co je potřeba procvičit.
4. **Studijní doporučení:** Vždy konkrétní — ne „procvičit geometrii", ale „procvičit výpočet obvodu a obsahu složených tvarů z více útvarů".
5. **Tón a délka zpětné vazby:** Řídit se preferencemi z „Kontext studenta" — pokud student chce stručnou zpětnou vazbu, nepsat romány. Pokud chce podrobné vysvětlení, vysvětli každý krok. Pokud chce motivační tón, přidej povzbuzení. Pokud preferuje věcný přístup, vynech ho.
6. **Jazyk:** Vždy česky. Technické termíny taktéž česky.
7. **Progres:** Při každém dalším testu srovnej výsledek s předchozím a okomentuj trend (zlepšení, stagnace, regrese v konkrétních oblastech).
8. **Nekombinuj odhady:** Pokud nelze jednoznačně přečíst studentovu odpověď, uveď to explicitně a vysvětli, co jsi přečetl.

---

## Studijní plán mezi testy

Po každé analýze navrhni **konkrétní studijní plán do příštího testu** v tomto formátu:

```markdown
## Studijní plán — po testu [kód testu]

### Priorita 1 (nejdůležitější slabé místo)
- **Oblast:** ...
- **Co konkrétně procvičit:** ...
- **Doporučená cvičení:** ...
- **Odhadovaný čas:** X hodin

### Priorita 2
- ...

### Co neměnit (silné oblasti)
- ... — v pořádku, stačí udržovat
```

Plán ulož do subfolderů posledního testu jako `Studijni_plan.md`.

---

## CERMAT — struktura testů (čtyřleté gymnázium)

### Matematika a její aplikace — 50 bodů, 70 minut

Úlohy 1–10: otevřené úlohy (postup řešení)
Úlohy 11–26: uzavřené (výběr z možností, přiřazování, ano/ne)

| Oblast | Typická váha |
|--------|-------------|
| Čísla a početní operace | ~20 % |
| Algebra (výrazy, rovnice, nerovnice) | ~20 % |
| Geometrie (rovinná + prostorová tělesa) | ~25 % |
| Slovní úlohy a kombinatorika | ~20 % |
| Statistika a pravděpodobnost | ~15 % |

### Český jazyk a literatura — 50 bodů, 60 minut

Testy zahrnují jeden nebo více textů (publicistický, umělecký, odborný). Úlohy testují práci s textem, jazykové znalosti a slovní zásobu.

| Oblast | Typická váha |
|--------|-------------|
| Porozumění textu (čtení s porozuměním) | ~40 % |
| Gramatika a pravopis | ~25 % |
| Syntax a stavba věty | ~20 % |
| Slovní zásoba a slohové prostředky | ~15 % |

**Časté typy úloh v češtině:**
- Určení hlavní myšlenky, záměru autora, postoje autora
- Doplnění správné podoby slova (skloňování, časování)
- Pravopis: i/y, s/z, velká písmena, interpunkce
- Určení větných členů, souvětí, druhu vedlejších vět
- Synonyma, antonyma, frazeologie

---

## Kontext studenta

**Jméno:** Adrian
**Datum onboardingu:** 27. 2. 2026

**Škola:** Velmi konkurenční (Praha centrum, Brno centrum, elitní školy)
**Cílové skóre:** 85+/100 (43+ bodů z 50 v každém předmětu)

**Sebehodnocení:**
- Matematika: 9–10 (velmi dobré)
- Čeština: 7–8 (docela dobře, složitější jevy)
- Typ chyb: Chybí látka (neznám postup nebo vzorec)

**Příprava:**
- Čas: 2–5 hodin týdně
- Způsob: Sám, bez doučování
- Přístup k testům: Ano, stahuje z cermat.cz nebo Scio

**Preference zpětné vazby:**
- Délka: Podrobně — vysvětlení každé chyby krok po kroku
- Tón: Věcný — jen fakta, bez zbytečných komentářů

---

## Dosavadní slabé oblasti

*Tuto sekci aktualizuj po každém testu.*

### Matematika
— (doplnit po prvním testu)

### Český jazyk
— (doplnit po prvním testu)

---

## Přehled testů

*Aktuální přehled viz `README.md` → tabulka „Přehled testů".*
