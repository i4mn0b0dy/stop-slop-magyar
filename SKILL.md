---
name: "stop-slop-magyar"
description: "Magyar próza szerkesztése: töltelékszavak, terpeszkedő kifejezések, óvatoskodó felvezetők és tükörfordítások kigyomlálása. Akkor használandó, amikor a feladat magyar szöveg írása, szerkesztése, lektorálása, tömörítése vagy AI-szagának eltüntetése. Use when writing, editing, proofreading or de-slopping Hungarian prose."
---

# Stop Slop – magyar

Magyar prózából gyomláld ki az AI-szagú és tükörfordítás-ízű fordulatokat. A `stop-slop` (Hardik Pandya, MIT) magyar viszonyokra hangolt párja. Használd, amikor magyar szöveget írsz, szerkesztesz vagy lektorálsz. A cél emberi, gördülékeny folyószöveg: közvetlen, cselekvő, konkrét, változatos ritmusú.

## Mikor ne használd

- **Jogi, hatósági, szerződéses szöveg**, ahol a forma kötött. Ott a terpeszkedő szerkezet gyakran előírás, nem hiba.
- **Idézet, interjúrészlet, forrásszöveg.** Más szavát ne írd át. Ha a szöveg idézeteket tartalmaz, csak a körülötte lévő saját prózát szerkeszd.
- **Szépirodalom, vers, dalszöveg, szándékosan archaizáló vagy ironikus stílus.**
- **Kód, változónevek, API-mezők, parancsok, tulajdon- és márkanevek.**
- **Nem magyar szöveg.** Ez a skill csak magyar prózára való.

## Munkamenet

1. Nézd át a szöveget, és jelöld ki, mi nem szerkeszthető (idézet, jogi rész, kód). Azt hagyd érintetlenül.
2. Menj végig a lenti gyors ellenőrzésen.
3. Írd át. A jelentést ne változtasd meg: ha a tömörítés tényt vagy árnyalatot venne el, maradjon a hosszabb változat.
4. Így add vissza az eredményt:
   - **Átírt szöveg** — csak a kész szöveg, kommentár nélkül.
   - **Változtatások** — legfeljebb 8 pont, „eredeti → új (miért)" formában. A gépies cseréket ne sorold fel egyenként.
   - **Kérdések** — ha valamit jelentésvesztés nélkül nem tudtál átírni, kérdezd meg.
5. Ha a felhasználó csak véleményt kért („mi a baj ezzel a szöveggel?"), ne írd át: sorold fel a hibákat, és pontozz.

## Alapelvek

1. **Töröld a tölteléket.** Vágd ki az üres határozószókat, az óvatoskodó felvezetőket és a nyomatékosító panelmondatokat.
2. **Bontsd fel a terpeszkedő kifejezéseket.** A főnevesített szerkezet helyett használj igét: „javításra kerül" → „megjavítják", „döntést hoz" → „dönt".
3. **Cselekvő szerkezet, valódi alannyal.** Kerüld a „megállapítható, hogy", „elmondható, hogy" típusú személytelen körülírást. Nevezd meg, ki mit tesz.
4. **Konkrétság.** Ne írd, hogy valami „fontos", „jelentős" vagy „strukturális" — nevezd meg pontosan. Kerüld a „minden", „mindig", „soha" üres túlzásait.
5. **Tükörfordítás-mentesség.** Az angolból szó szerint átvett fordulatokat cseréld magyar megfelelőre (lásd lista lentebb).
6. **Változatos ritmus.** Váltogasd a mondathosszt. Ne halmozz rövid, pattogó tőmondatokat. A bekezdések ne mind csattanóval végződjenek.
7. **Bízz az olvasóban.** Ne magyarázd túl, ne kérj engedélyt, ne ismételd el a saját mondanivalódat.
8. **Idegen szó helyett magyar,** ha van jó megfelelő: implementál → megvalósít, fókuszál → összpontosít, releváns → fontos/idevágó, preferál → előnyben részesít. (A meghonosodott szakszót zárójeles magyarázattal meghagyhatod.)

## Gyors ellenőrzés (mielőtt leadod)

- Van benne üres határozószó (valójában, gyakorlatilag, tulajdonképpen, lényegében, alapvetően)? Töröld.
- Terpeszkedő kifejezés („intézkedést hoz", „vizsgálat alá vet", „-ásra/-ésre kerül")? Cseréld igére.
- Személytelen körülírás („elmondható, hogy", „megállapítható")? Nevezd meg az alanyt.
- Óvatoskodó felvezető („Fontos megjegyezni, hogy", „Érdemes szem előtt tartani")? Vágd ki, mondd a lényeget.
- Tükörfordítás („a nap végén", „amikor a ...-ról van szó", „egy olyan világban, ahol")? Cseréld magyar fordulatra.
- Halmozott „az, hogy" / „azt, hogy"? Fogalmazd át.
- Birtokos lánc („a cég vezetőjének a döntésének a hatása")? Bontsd szét.
- Három tagú felsorolás pusztán a ritmusért? Vedd kettőre.
- Sok egymást követő mondat „Tehát" / „Illetve" / „Azonban" kezdéssel? Változtass.
- Csattanó egymondatos bekezdészárás minden bekezdésben? Váltogasd.

## Kerülendő szavak és fordulatok

**Üres határozószók, töltelékek** (töröld): valójában, gyakorlatilag, tulajdonképpen, lényegében, alapvetően, kifejezetten, rendkívül, hihetetlenül, egyszerűen (csak), tényleg, őszintén (szólva), voltaképpen, jószerével. Panelek: „ami azt illeti", „az igazság az, hogy", „valljuk be", „lássuk be", „a mai rohanó világban", „napjainkban", „a modern világban".

**Óvatoskodó / AI-felvezetők** (vágd ki, mondd a lényeget): „Fontos megjegyezni, hogy", „Érdemes megjegyezni/szem előtt tartani, hogy", „Ne feledd(kezzünk meg arról), hogy", „Fontos hangsúlyozni, hogy", „Meg kell említeni, hogy", „Íme", „Nézzük (meg)", „Lássuk", „Beszéljünk arról, hogy", „Az alábbiakban", „Ebben a részben".

**Tükörfordítás angolból** (bal → jobb): „a nap végén" → a lényeg / végső soron; „amikor a ...-ról van szó" → a ...-ban / ...-nál; „egy olyan világban, ahol" → (töröld, mondd konkrétan); „nemcsak X, hanem Y is" → X is, Y is (ha nem drámai kontraszt); „ez azt jelenti, hogy" → gyakran törölhető; „a helyzet az, hogy" → (töröld); „a végén" (at the end) → végül.

**Bürokratikus / hivataloskodó fordulatok**: „...-val/-vel kapcsolatban" → ...-ról; „...vonatkozásában / tekintetében" → ...-ban / ...-nál; „annak érdekében, hogy" → hogy; „azzal a céllal, hogy" → hogy; „a fentiek alapján" → ezért.

**Megalapozatlan általánosítás**: a „minden", „mindig", „soha", „mindenki", „senki", „teljesen", „tökéletesen" akkor hiba, ha csak nyomatéknak használod. „Minden felhasználó ezt akarja" → „a megkérdezett tizenkettőből kilenc ezt akarta". Ha az állítás kivétel nélküli, maradhat.

## Terpeszkedő kifejezések (fő magyar hiba)

A magyar AI-szöveg leggyakoribb jele: az igét főnév + segédige párosra bontja. Cseréld vissza igére.

- „döntést hoz" → dönt
- „intézkedést hoz / foganatosít" → intézkedik
- „javításra kerül" → megjavítják
- „megvalósításra kerül" → megvalósul / megvalósítják
- „használatra kerül" → használják
- „vizsgálat alá vet" → megvizsgál
- „figyelembevételre kerül" → figyelembe veszik
- „alkalmazásra kerül" → alkalmazzák
- „elvégzi a ... folyamatát" → egyszerűen: ...

Ökölszabály: ha egy mondatban „-ás/-és + kerül / hoz / végez / eszközöl", ott terpeszkedő kifejezés lapul.

## Szerkezeti hibák

**Bináris kontraszt** (magyarban is gépies, ha halmozod): „Nem X. Hanem Y.", „Nem arról van szó, hogy X, hanem hogy Y", „A kérdés nem az, hogy X, hanem hogy Y". Ritkán, hangsúlyért még rendben — de alapból mondd ki Y-t közvetlenül.

**Személytelen körülírás** (nevezd meg a cselekvőt): „elmondható, hogy", „megállapítható, hogy", „kijelenthető, hogy", „az a helyzet áll fenn, hogy", „arra a következtetésre lehet jutni". Helyette: ki mondja, ki állapítja meg, ki dönt.

**Elbújtatott cselekvő**: ha számít, ki cselekszik, ne rejtsd el. „A tanulmány azt javasolja" → „a szerzők azt javasolják"; „a kultúra megváltozik" → „a vezetők megváltoztatják". Ha a cselekvő lényegtelen, maradhat: „az adatok azt mutatják" és „megszületett a döntés" jó magyar fordulat, nem kell irtani.

**Kötőszó-tapadás**: sok mondat „Tehát", „Illetve", „Valamint", „Azonban", „Ugyanakkor" kezdéssel. Ritkítsd, változtass.

**„az, hogy" halmozás**: „Az a fontos, hogy tudjuk, hogy az a cél, hogy..." — bontsd szét, fogalmazd újra.

## Példák

Előtte: „A csapat elvégezte a hiba javításának a folyamatát, aminek eredményeként a rendszer működőképessé vált."
Utána: „A csapat megjavította a hibát, és a rendszer újra működött."

Előtte: „A nap végén tulajdonképpen az a helyzet áll fenn, hogy a megtakarítás valójában a legfontosabb tényező."
Utána: „A megtakarítás a legfontosabb."

Előtte: „Fontos megjegyezni, hogy nem arról van szó, hogy a tudás számít, hanem sokkal inkább arról, hogy a viselkedés."
Utána: „A viselkedés számít, nem a tudás."

Előtte: „A megoldás implementálása kapcsán érdemes szem előtt tartani a felhasználói élmény optimalizálásának a fontosságát."
Utána: „A megoldásnál a felhasználókra kell figyelnünk."

Előtte: „Egy olyan világban, ahol minden gyorsan változik, napjainkban rendkívül fontos a rugalmasság."
Utána: „Ma a rugalmasság dönt."

## Pontozás

Akkor pontozz, ha a felhasználó értékelést, visszajelzést vagy összehasonlítást kér. A sima átírás mellé ne tedd oda magadtól.

Öt szempont, egyenként 1–10: Közvetlenség (kimond vagy bejelent?), Ritmus (változatos vagy gépies?), Cselekvőség (van valódi alany, ige?), Természetesség (magyaros, emberi hangzású?), Tömörség (van kihúzható szó?). Add meg az öt számot, az összeget, és szempontonként egy mondat indoklást. 35/50 alatt: át kell dolgozni.

