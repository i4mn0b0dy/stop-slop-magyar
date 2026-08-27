# Tesztesetek

Futtató nincs hozzá. Add oda a kérést egy Claude-példánynak előbb a skill nélkül, aztán a skillel. Ha a skill nélküli válasz is teljesíti a feltételeket, az a szabály nem old meg semmit — vedd ki.

A harmadik teszt a legfontosabb. Ott nem azt mérjük, kigyomlálja-e a hibákat, hanem azt, hogy békén hagyja-e, amihez nem szabad nyúlnia.

## 1. Hivataloskodó körlevél

> Írd át ezt a belső körlevelet olvashatóra:
>
> „Tájékoztatjuk a Tisztelt Munkatársakat, hogy a rendszer karbantartása vonatkozásában a jövő héten intézkedés kerül foganatosításra. A leállás időpontja a fentiek alapján még pontosításra kerül, azonban elmondható, hogy a munkavégzést várhatóan nem befolyásolja. Annak érdekében, hogy a folyamat zökkenőmentes legyen, kérjük, hogy a mentések elvégzésének a folyamatát mindenki hajtsa végre. Fontos megjegyezni, hogy a hozzáférési jogosultságok felülvizsgálat alá vetésre kerülnek."

Átmegy, ha:

- a terpeszkedő szerkezetek igére váltanak: „intézkedés kerül foganatosításra" → karbantartjuk, „felülvizsgálat alá vetésre kerülnek" → felülvizsgáljuk;
- az „elmondható, hogy" helyett megnevezi a cselekvőt;
- kiesik a „Fontos megjegyezni, hogy", az „annak érdekében, hogy" és a „fentiek alapján";
- megmarad mind a négy tény: jövő heti karbantartás, még nincs időpont, mentéskérés, jogosultság-felülvizsgálat;
- a formátum stimmel: átírt szöveg, aztán a változtatások listája;
- nem pontoz, mert a felhasználó nem kért értékelést.

## 2. AI-szagú marketingszöveg

> Mi a baj ezzel a szöveggel?
>
> „Egy olyan világban, ahol minden nap gyorsabban változik, a mai rohanó világban tulajdonképpen mindenki keresi a megoldást. A nap végén az igazság az, hogy nem a technológia számít. Hanem az ember. Fontos megjegyezni, hogy amikor a digitális átalakulásról van szó, a kérdés nem az, hogy változtatunk-e, hanem hogy mikor. Platformunk implementálása kapcsán érdemes szem előtt tartani a felhasználói élmény optimalizálásának a fontosságát. Egyszerű. Gyors. Hatékony."

Átmegy, ha:

- nem írja át, mert véleményt kértek, nem szerkesztést;
- megnevezi a tükörfordításokat és a töltelékeket;
- szóvá teszi a halmozott bináris kontrasztot és a záró „Egyszerű. Gyors. Hatékony." tőmondatsort;
- pontoz, mert értékelést kértek, és 35/50 alatt marad.

## 3. Idézet és szerződés — ehhez ne nyúljon

> Gyomláld ki ebből a cikkrészletből az AI-szagot:
>
> „A cég tegnap bejelentette az átszervezést. Fontos megjegyezni, hogy a döntés meghozatalára hosszú egyeztetés után került sor, és a nap végén tulajdonképpen mindenki elfogadta.
>
> Kovács Anna, a szakszervezet vezetője így fogalmazott: »Elmondható, hogy a munkavállalók érdekei figyelembevételre kerültek, ugyanakkor a folyamat átláthatósága vonatkozásában továbbra is vannak fenntartásaink.«
>
> A szerződés 4.2 pontja szerint: »A Felek rögzítik, hogy a jelen szerződés alapján teljesítendő szolgáltatások vonatkozásában a Megrendelő részéről kifogás előterjesztésére a teljesítéstől számított 30 (harminc) napon belül kerülhet sor.«
>
> Az átszervezés a jövőben érinti a budapesti telephelyet is."

Átmegy, ha:

- az idézet szó szerint marad, pedig tele van terpeszkedő és személytelen szerkezettel;
- a szerződés 4.2 pontja szó szerint marad;
- a név és a 30 napos határidő változatlan;
- a saját újságírói prózát viszont átírja;
- a „mindenki elfogadta" nem cserélődik kitalált számadatra;
- jelzi, hogy az idézetet és a szerződéses részt szándékosan hagyta érintetlenül.
