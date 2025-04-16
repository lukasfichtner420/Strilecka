# Dokumentace k hernímu projektu

**Autor:** Lukáš Fichtner  
**Název hry:** Top-down střílečka

---

## 1. Základní koncepce

Hra je 2D top-down střílečka vytvořená v herním enginu **Godot 4**.  
Hráč ovládá postavu z ptačí perspektivy a střílí nepřátele, kteří se na něj vrhají ze všech stran.  
Základem hratelnosti je svižný pohyb, rychlá střelba a nutnost vyhýbat se nepřátelům. Nepřátelé se objevují náhodně, stejně tak se generují stěny, které vytvářejí překážky v prostoru.

**Technologie:**
- Herní engine: Godot 4
- Jazyk: GDScript
- Architektura: scény pro hráče, nepřátele, střely, výbuchy, překážky, hlavní scéna hry

---

## 2. GameDesign

**Pravidla:**
- Hráč má neomezený počet životů, ale po kolizi s nepřítelem se hra restartuje.
- Střely se pohybují směrem, kterým hráč míří myší.
- Nepřátelé jdou vždy směrem k hráči.

**Objekty a atributy:**

| Objekt     | Atributy                            |
|------------|-------------------------------------|
| Hráč       | Rychlost: 200                       |
| Střela     | Rychlost: 10, směr střelby, životnost  |
| Nepřítel   | Rychlost: 100                       |
| Stěna      | Statická překážka                   |

**Prostředí:**
- Herní pole obsahuje náhodně generované stěny (rozmístění a velikost).
- Nepřátelé se spawnují v určité vzdálenosti od hráče, aby se zabránilo nespravedlivému útoku.

---

## 3. Grafika

**Styl:** 2D minimalistický styl  
**Formát:** Pixelart / barevné tvary  
**Použité nástroje:**  
- Zatím použity jednoduché barvy a obdélníky přímo v Godotu (`ColorRect`, `Sprite2D`)  
- Ve finální verzi lze doplnit vlastní grafiku nebo sprity

---

## 4. Zvuky

Zatím nejsou přidány zvukové efekty.  
Ve finální verzi se plánuje použití softwaru jako **Audacity** k tvorbě vlastních zvuků (např. výstřel, výbuch, zásah).

---

## 5. Hudba

Hudba zatím není přidána.  
Plán: vytvořit jednoduchý smyčkový podkres v nástroji **LMMS**, např. elektronický ambientní motiv.

---

## 6. Implementace

**Hotové prototypy:**
- Pohyb hráče pomocí `CharacterBody2D`
- Směřování pohledu k myši
- Střelba a kolize střely s nepřítelem a stěnou
- Spawnování nepřátel ve vzdálenosti od hráče
- Náhodné generování stěn

Hra je funkční v základní podobě.

---

## 7. Propagace

Propagační materiály zatím nevytvořeny.  
Plán: jednoduché gameplay video a krátké gif ukázky přímo ze hry.

---

## 8. Finální hra

Verze odevzdané hry obsahuje:
- Funkční základní herní smyčku (pohyb, střelba, nepřátelé)
- Náhodně generované překážky
- Restart hry po smrti hráče

Chybí zvukové a hudební prvky, pokročilá grafika a menu.

---

## 9. Závěr

Při vývoji jsem narazil na několik technických komplikací. Nejsložitější bylo správné nastavení kolizí mezi různými objekty a generování stěn tak, aby neblokovaly hráče od začátku.

---

## ❗ Omluva

Velmi se omlouvám panu učiteli.  
Měl jsem problém s počítačem – po spuštění Godotu mi opakovaně naskakoval **modrý displej smrti (Blue Screen)**. Kvůli tomu jsem nestihl projekt plně dokončit v plánovaném rozsahu.

Odevzdávám proto **ne zcela hotovou, ale funkční hru**, kde je možné si vyzkoušet hlavní herní mechaniky.  
Děkuji za pochopení.

**Autor:** *Lukáš Fichtner*
