# provenzanodj.com

Sito di Provenzano Dj, pubblicato con **GitHub Pages**: ogni push su `main` va online da solo.
Grafica nella direzione D (nero `#000`, rosso `#FF3131`, Anton maiuscolo, il punto del logo come
firma); il sito vero cresce pezzo per pezzo sullo stesso repo.

La home non dice più "in costruzione" (tolto il 20/08/2026): sotto il logo c'è **Crossover**,
che porta a `/crossover/puntate/`, poi la riga dei trent'anni, poi un solo *Scrivimi* con i tre
indirizzi. La regola è quella: la home mostra la cosa che il sito ha davvero, non la promessa di
quella che avrà.

Brief, decisioni e archivio del progetto: `02-PROVENZANO-DJ/sito/` nel workspace privato
(`apalmix70/provenzano-workspace`). Questo repo contiene **solo** ciò che va online.

- `index.html` — la home, senza build: si modifica e si pusha. Le quattro voci in colonna
  sono, in quest'ordine: **Biografia, Discografia, Compilation, Crossover** (Amerigo, 03/09/2026)
- `biografia/` — la storia in prima persona, dal 1970 a oggi. **Scritta a mano, non generata**:
  è testo, si modifica direttamente qui. Le fonti e le regole di voce stanno nel workspace
  privato (`context/chi-sono.md` e `02-PROVENZANO-DJ/sito/brief.md`): prima persona,
  «tu» al visitatore, poche parole e molti fatti
- `crossover/` — l'archivio dei dischi passati in Crossover: `index.html` è la pagina di
  ricerca, `numeri/index.html` le statistiche, `dati/` i due JSON che le alimentano.
  **Non si modificano a mano**: sono generati dal workspace privato
  (`02-PROVENZANO-DJ/instagram/crossover/database/`, comando `python aggiorna.py`),
  che ogni settimana ci riversa la puntata nuova
- `foto/` — la figura della home. **Generata con GPT Image 2** (Higgsfield) partendo dalla
  foto di riferimento del volto, non ripresa da un servizio fotografico: total black su fondo
  nero, una sola luce rossa di taglio lungo il braccio. In pagina c'è `hero-v3.jpg`; le altre
  tre restano come alternative. ⚠️ **Il nero della foto è già portato a `#000` e i bordi sono
  già sfumati nel file** — è quello che la fa sparire dentro la pagina invece di lasciare un
  rettangolo visibile. Se si cambia foto va rifatto quel passaggio, non aggiunta una maschera
  CSS. Originali a piena risoluzione in `D:\VIDEO - PROVENZANO\sito\hero-home\`
- `fonts/` — Anton e Poppins ExtraBold (OFL)
- `icons/` — icone social da [simple-icons](https://simpleicons.org) (CC0)
- `CNAME` — arriverà quando il dominio Aruba viene puntato su GitHub Pages
