# ads-dashboard — HANDOFF per Claude

> Repo: `PrimaSorte/ads-dashboard`. Dentro c'è uno snapshot congelato di SGR System (Bquadro) + il contratto dati. Niente backend e niente RAG in questa fase: leggi solo `snapshot/`.

## Cosa devi costruire

Una parte **da advertiser dentro il tuo clone di TickTick**: stesso linguaggio, stessa app, una sezione nuova dove Luca prepara le ads. Non una dashboard separata, non un secondo stile: un pezzo del TickTick che stai già facendo.

## Cosa contiene lo snapshot

- **5 angoli (A1-A5)**: modi diversi di presentare lo stesso sistema. Ognuno ha: nome, hook (frase d'apertura), pain (problema), meccanismo (perché funziona), benefici, consapevolezza (quanto il pubblico conosce già il problema: L2 = sa di avere il problema, L3 = conosce già soluzioni), ondataTest (prima ondata = da testare subito, seconda ondata = dopo), provaNecessaria (quale prova serve prima di usare davvero quest'angolo), rischioDaEvitare (cosa non deve comunicare).
- **Claim gate**: 9 frasi vietate senza prova (percentuali, promesse, "unico al mondo"...). Sono il confine: quello che esce da qui dentro non deve mai contenerle.
- **Offerta ipotizzata + CTA provvisorie**: cosa si propone di offrire al lead, ancora da confermare col cliente.
- **Blocchi aperti**: le domande senza risposta (a Sergio/Matteo e a Luca/Viviana). Finché ci sono, niente è definitivo.
- **Landing**: solo puntatori (URL e ID documenti), non testo da pubblicare.
- Tutto è **bozza non approvata dal cliente**: si può progettare sopra, non pubblicare.

## Cosa deve fare la sezione advertiser

1. **Angoli**: le 5 card con tutto quello che dice lo snapshot, incluse prova necessaria, rischio e ondata. A3 vale solo se confermato il segmento multi-operatore.
2. **Nuova Ad**: Luca parte da 1-3 angoli e prepara un brief (formato, note). Il brief tiene insieme: da quali angoli viene, quali vincoli del claim gate valgono, cosa manca ancora.
3. **Claim gate + Blocchi**: sempre visibili prima di qualsiasi export.

## Cosa non deve mai succedere

- Numeri, percentuali, promesse, casi o nomi che non sono nello snapshot. In particolare mai: -70%, -55%, importi di risparmio, 24 ore, zero sprechi, "unico al mondo".
- Hook riscritti senza dirlo: o verbatim, o marcati `parafrasi`.
- Lo snapshot non decide al posto di Luca: mostra lenti e vincoli, lui sceglie.

## Contratto dati

`snapshot/schema.json`. Se un campo che ti serve manca, dillo a Luca e lo aggiungo io: non inventarlo tu. Quando il RAG dal vivo nutrirà lo stesso formato, la tua UI non cambia.
