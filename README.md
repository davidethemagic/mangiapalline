# Mangiapalline

Un gioco del labirinto con quattro fantasmi, in un solo file HTML. Mangi tutte le palline senza farti prendere; quelle grandi spaventano i fantasmi e per qualche secondo puoi mangiarli tu.

## Come si gioca

- Tastiera: frecce, oppure `W` `A` `S` `D`.
- Telefono: scorri il dito sul labirinto, oppure usa i tasti a schermo.
- `P` o `Spazio`: pausa e ripresa. Il gioco si mette in pausa da solo se cambi scheda.
- `M`: audio acceso o spento.

Hai tre vite. Il punteggio migliore resta salvato nel browser.

## Punteggi

| Cosa | Punti |
| --- | --- |
| Pallina | 10 |
| Pallina grande | 50 |
| Primo fantasma mangiato con una pallina grande | 200 |
| Fantasmi successivi con la stessa pallina | 400, 800, 1600 |

## I fantasmi

Ognuno ha un carattere diverso quando ti insegue:

- **Blinky** (rosso) ti viene dritto addosso. Quando restano poche palline diventa più aggressivo.
- **Pinky** (rosa) punta quattro caselle davanti a te, per tagliarti la strada.
- **Inky** (azzurro) sceglie la mossa guardando anche dove si trova Blinky.
- **Clyde** (arancione) ti insegue da lontano e scappa nel suo angolo quando ti avvicini.

I fantasmi alternano fasi in cui ti inseguono e fasi in cui tornano ai loro angoli. Un fantasma mangiato torna alla casa e riparte. A ogni livello i fantasmi escono più in fretta e corrono di più, e il tempo in cui sono spaventati si accorcia.

## Come funziona

- Il labirinto è una griglia di 19 per 21 caselle, descritta come testo nel codice. Si cambia modificando le righe.
- Il tunnel ai lati si attraversa: esci a sinistra e rientri a destra.
- Il percorso del fantasma mangiato verso la casa è calcolato con una ricerca in ampiezza.
- Il disegno è tutto su un canvas, nitido anche sugli schermi ad alta densità.
- I suoni sono generati dal browser, non ci sono file audio.

## Provarlo

È un solo file, `index.html`. Scaricalo e aprilo nel browser: non serve installare niente. L'unica cosa che scarica dalla rete sono i caratteri di Google Fonts; se è offline il gioco funziona lo stesso con quelli di sistema.

## Licenza

MIT. Puoi usarlo, copiarlo e modificarlo come vuoi.
