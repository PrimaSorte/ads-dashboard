# ads-dashboard — HANDOFF per Claude

> Repo: `PrimaSorte/ads-dashboard`. Dati: `snapshot/sgr-snapshot.json`. È una demo statica: niente backend, niente generazione immagini, niente pubblicazione.

## Cosa devi costruire

Una sezione **da advertiser dentro il tuo clone di TickTick**: stesso linguaggio, stessa app. È un prototipo semplice, una sola area di lavoro notion-like che mescola due cose:

- **vista a task**: la lista di quello su cui Luca sta lavorando (i 3 angoli della prima ondata: A1, A2, A3);
- **tessere operative**: card con dentro gli swipe file, cioè per ogni angolo il suo hook e il suo meccanismo, pronti da guardare mentre si lavora.

Pensa a Notion: metà lista di task, metà tessere consultabili. Niente di più per ora: niente builder, niente export, niente claim gate, niente blocchi, niente immagini generate.

## Dati da usare (solo questi)

Dallo snapshot, solo l'array `angles`. Per ogni angolo ti servono: `code`, `name`, `hook`, `pain`, `mechanism`. Ignora tutto il resto del file in questa fase.

## Cosa non deve mai succedere

- Generare immagini o finti visual.
- Aggiungere numeri, promesse, casi o testi che non sono nello snapshot.
- Riscrivere gli hook senza dirlo: o verbatim, o marcati `parafrasi`.

## Contratto dati

`snapshot/schema.json`. Se un campo ti serve e manca, dillo a Luca: lo aggiungo io, non inventarlo tu.
