# stop-slop-magyar

Claude-skill, amely az AI-szagú és tükörfordítás-ízű fordulatokat gyomlálja ki a magyar prózából: töltelékszavak, terpeszkedő kifejezések, óvatoskodó felvezetők, anglicizmusok.

A [stop-slop](https://github.com/hardikpandya/stop-slop) (Hardik Pandya, MIT licenc) magyar párja. A szabályok a magyar szövegek saját hibáira épülnek: terpeszkedő szerkezetek, bürokratikus fordulatok, tükörfordítások.

## Mit csinál

Amikor Claude magyar szöveget ír, szerkeszt vagy lektorál, ez a skill arra tanítja, hogy:

- vágja ki az üres határozószókat és panelmondatokat,
- bontsa fel a terpeszkedő kifejezéseket igékre (pl. „döntést hoz" → „dönt"),
- használjon cselekvő szerkezetet valódi alannyal,
- legyen konkrét absztrakciók helyett,
- cserélje le a tükörfordításokat magyar fordulatokra,
- változatos mondatritmust tartson.

Azt is megmondja, mikor **ne** nyúljon a szöveghez: idézetet, jogi és szerződéses részt, verset, kódot érintetlenül hagy.

A `SKILL.md` tartalmazza a munkamenetet, a teljes szabálylistát, a leadás előtti gyors ellenőrzőlistát és előtte/utána példákat.

## Telepítés

Másold a `SKILL.md`-t a saját Claude-skill mappádba:

```
mkdir -p ~/.claude/skills/stop-slop-magyar
cp SKILL.md ~/.claude/skills/stop-slop-magyar/
```

A mappa nevének egyeznie kell a `SKILL.md` frontmatterében szereplő `name` mezővel (`stop-slop-magyar`), különben a skill nem töltődik be.

(Az elérési út a Claude-kliens szerint eltérhet — Claude Code-nál, Cowork-nél vagy claude.ai-nál más-más helyre kerülnek a felhasználói skillek.)

## Tesztelés

Ha módosítod a szabályokat, egy dolgot ellenőrizz újra: adj a skillnek egy cikkrészletet, amelyben idézet és szerződéses bekezdés is van, mindkettő tele terpeszkedő szerkezettel. Ha bármelyikhez hozzányúl, a „Mikor ne használd" rész nem elég erős.

## Licenc

MIT — lásd [LICENSE](LICENSE). Az eredeti `stop-slop` szintén MIT licenc alatt áll.
