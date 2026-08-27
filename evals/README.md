# Evals

Három forgatókönyv a skill ellenőrzésére. Nincs hozzá futtató — kézzel kell lefuttatni, de a lényeg az összehasonlítás:

1. **Alapvonal:** add oda a `query` szövegét egy Claude-példánynak a skill **nélkül**. Írd le, mit csinál.
2. **Skillel:** ugyanaz a kérés, betöltött skillel.
3. **Értékelés:** teljesül-e az `expected_behavior` minden pontja. Ha a skill nélküli futás is teljesíti mindet, az a szabály nem old meg valós problémát.

A 03-as forgatókönyv negatív teszt: ott a skill **túlkapását** méri. Ha a modell átírja a jogi bekezdést vagy az idézetet, a skill „Mikor ne használd" része nem elég erős.

Érdemes mindhármat Haikuval, Sonnettel és Opusszal is végigfuttatni — a szűkszavú szabályok kisebb modelleken másképp sülnek el.
