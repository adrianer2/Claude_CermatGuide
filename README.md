# Claude_CermatGuide
Tohle je claude "work in a folder" cowork, kde si uploadneš testy, claude to analyzuje, a dává ti velmi užitečnou zpětnou vazbu, já jsem se s tímto vyšplhal z 51 bodů z matiky a češtiny spolu, na průměrně 86 bodů spolu

# Příprava na přijímací zkoušky s AI asistentem

Workspace pro přípravu na přijímací zkoušky na gymnázium (CERMAT). Claude funguje jako osobní tutor — zpracuje tvoje odpovědi z testu, opraví je, vysvětlí každou chybu a navrhne, co procvičit dál.

---

## Jak to funguje

Celé chování AI je definované souborem `CLAUDE.md` v kořeni složky. Když Claude otevře tento workspace, přečte soubor a ví, co má dělat — jaké otázky se zeptat, jak analyzovat test, kam uložit výsledky, v jakém formátu psát zpětnou vazbu.

Žádný kód. Jen textové soubory.

```
CLAUDE.md        ← instrukce pro AI (co dělat, jak se chovat, jaké šablony použít)
README.md        ← tento soubor
Matematika/      ← sem se ukládají testy a analýzy z matiky
Cesky jazyk/     ← totéž pro češtinu
```

---

## Použití

### Co potřebuješ

- [Claude desktop app](https://claude.ai/download) s Cowork modem (research preview)
- Testy z minulých let — stáhneš zdarma na [prijimacky.cermat.cz](https://prijimacky.cermat.cz)

### Jak začít

1. Stáhni nebo naklonuj tento repozitář
2. Otevři Claude desktop a vyber tuto složku jako workspace
3. Napiš cokoli — Claude se sám představí a provede tě nastavením

### Jak přidat nový test

1. Stáhni PDF se zadáním testu z cermat.cz
2. Vyplň test na papíře nebo v PDF
3. Vyfoť nebo udělej screenshot svých odpovědí
4. Nahraj soubory do chatu a napiš: *„Analyzuj tento test z matematiky"*
5. Claude opraví test, spočítá skóre, vysvětlí každou chybu a uloží výsledky do složky

---

## Co Claude udělá automaticky

- Při prvním spuštění provede onboarding — zeptá se na cílovou školu, sebehodnocení, časové možnosti a preferovaný styl zpětné vazby
- Výsledky každého testu uloží do strukturované složky (`RRRR-MM-DD_<kód_testu>/`)
- Po každém testu aktualizuje přehled výkonu a navrhne konkrétní studijní plán
- Při dalším testu porovná výsledky a okomentuje trend

---

## Jak navrhnout vlastní workspace takhle

Princip je přenositelný na jakýkoli jiný projekt:

1. Vytvoř složku
2. Přidej `CLAUDE.md` — napiš do něj, co má AI dělat, na co se ptát, jak strukturovat výstupy
3. Otevři složku v Claude Cowork
4. Hotovo — AI čte soubor a chová se podle něj

`CLAUDE.md` je v podstatě systémový prompt pro konkrétní workflow, uložený jako součást projektu.

