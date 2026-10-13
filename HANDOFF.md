# ads-dashboard — HANDOFF per Claude

> Repo: `PrimaSorte/ads-dashboard`. Contenuto: snapshot SGR congelato + contratto. Niente backend, niente Vault, niente RAG in questa fase.

## Cosa hai davanti

- `snapshot/sgr-snapshot.json` — l'unico dato. Angoli A1-A5, claim gate, offerta ipotizzata, CTA provvisorie, diagnosi, landing (solo puntatori), blocchi aperti. Tutto marcato bozza: **non è copy approvato dal cliente**.
- `snapshot/schema.json` — il contratto. Se un giorno il JSON viene nutrito dal vivo, il formato resta questo e la tua UI non cambia di una riga.

## Regole di design

- Riusa il linguaggio del tuo TickTick custom (dark, hairline, italiano). Non inventare un secondo stile.
- Una vista alla volta, con screenshot prima/dopo come stai già facendo.

## Goal in ordine (uno alla volta, fermati e mostra)

1. **Vista Angoli**: 5 card A1-A5 (nome, hook, pain, meccanismo, benefici, stadio, ondata). Badge visibile su `proofNeeded` e `risk` di ogni angolo. A3 marcata "solo se confermato segmento multi-operatore".
2. **Vista Nuova Ad**: builder di brief che parte da 1 angolo (lente dichiarata, max 3) + formato + note. Il brief mostra sempre: lenti usate, claim gate applicabile, cosa manca (blockers). Non genera copy finale: prepara il brief.
3. **Vista Claim gate + Blocchi**: le 9 frasi vietate senza prova e le domande aperte per Sergio/Matteo e Luca/Viviana, sempre visibili prima di qualsiasi export.

## Regole non-biasing (invalicabili)

- Hook e claim solo verbatim dallo snapshot. Se parafrasi, marca `parafrasi`.
- Mai numeri, percentuali, promesse o casi che non sono nello snapshot. In particolare mai: -70%, -55%, importi di risparmio, 24 ore, zero sprechi, "unico al mondo".
- Lo snapshot non decide al posto dell'utente: propone lenti e vincoli, la decisione resta a Luca.
- Niente chiamate di rete, niente backend, niente scrittura fuori dal repo. Leggi solo `snapshot/`.

## Il rubinetto dal vivo

Lo attacco io dopo: stesso JSON, nutrito dal RAG documentale. Il tuo lavoro non si rompe perché il contratto non cambia. Se un campo che ti serve manca, dimmelo e lo aggiungo io allo snapshot, non inventarlo tu.
