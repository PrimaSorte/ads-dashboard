# ads-dashboard — HANDOFF per Claude

> Repo: `PrimaSorte/ads-dashboard`. Dati: `snapshot/sgr-snapshot.json`. Demo statica, solo lettura dallo snapshot.

## Cosa devi costruire

Una sezione **da advertiser dentro il tuo clone di TickTick**: stesso linguaggio, stessa app. È un'area di lavoro notion-like che mescola vista a task e tessere consultabili: la lista di quello su cui Luca sta lavorando (i 3 angoli della prima ondata: A1, A2, A3) e, accanto, tessere con dentro gli swipe file di ogni angolo (hook e meccanismo, pronti da guardare mentre si lavora).

## I default dell'area

Come TickTick ha note e template di task con default, anche quest'area ha i suoi, così lo stesso scheletro potrà creare altre aree di lavoro in futuro:

- **tessera di default**: ogni tessera ha codice, nome, hook, problema e meccanismo;
- **task di default**: ogni task è collegato a una tessera e ha uno stato di lavorazione.

Quando costruisci, tieni separati lo scheletro (vista task + tessere + default) dai contenuti SGR: lo scheletro dovrà poter ospitare altre aree dopo questa.

## Dati da usare

Dallo snapshot, solo l'array `angles`. Per ogni angolo: `code`, `name`, `hook`, `pain`, `mechanism`.

## Testi

Solo testi dallo snapshot. Hook riscritti solo se marcati `parafrasi`.

## Contratto dati

`snapshot/schema.json`. Se un campo ti serve e manca, dillo a Luca: lo aggiungo io, non inventarlo tu.
