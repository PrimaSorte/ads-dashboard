# ads-dashboard — HANDOFF per Claude

> Repo: `PrimaSorte/ads-dashboard`. Dati: `snapshot/sgr-snapshot.json`. Demo statica, solo lettura dallo snapshot.

## Cos'è SGR

Leggi il campo `contesto` dello snapshot: è tutto quello che ti serve per sapere di cosa si parla.

## Cosa devi costruire

Una sezione **da advertiser dentro il tuo clone di TickTick**: stesso linguaggio, stessa app. È un'area di lavoro notion-like che mescola vista a task e tessere consultabili: la lista di quello su cui Luca sta lavorando (i 3 angoli della prima ondata) e, accanto, tessere con dentro gli swipe file di ogni angolo (hook e formato, pronti da guardare mentre si lavora).

## I default dell'area

Come TickTick ha note e template di task con default, anche quest'area ha i suoi, così lo stesso scheletro potrà creare altre aree di lavoro in futuro:

- **tessera di default**: ogni tessera ha nome, hook, problema e formato;
- **task di default**: ogni task è collegato a una tessera e ha uno stato di lavorazione.

## Per chi è quest'area

Il cliente è **Bquadro Astidental** (campo `cliente`); **SGR System** è l'offerta su cui fa le ads (campo `offerta`). Le ads avranno altri sottoclienti dopo questo: costruisci i contenitori (lista task + tessere + default) in modo che domani possano ospitare altri contenuti oltre SGR, senza rifarli.

## Come si chiama ciò che esce

Leggi il campo `naming` dello snapshot: la catena è Offerta → Angolo → Headline → Creatività numerate, e il nome segue il template `[OFFERTA]_[ANGOLO]_[HEADLINE]_[FORMATO]-[ITERAZIONE]`. Le tessere e i task usano gli stessi nomi.

## Dati da usare

Dallo snapshot: `contesto` e l'array `angles`. Per ogni angolo: `name`, `hook`, `pain`, `formato`. Il formato è ancora "da definire": mostralo come slot vuoto, non inventarlo.

## Testi

Solo testi dallo snapshot. Hook riscritti solo se marcati `parafrasi`.

## Contratto dati

`snapshot/schema.json`. Se un campo ti serve e manca, dillo a Luca: lo aggiungo io, non inventarlo tu.
