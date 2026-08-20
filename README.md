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

- `index.html` — la home, senza build: si modifica e si pusha
- `crossover/` — l'archivio dei dischi passati in Crossover: `index.html` è la pagina di
  ricerca, `numeri/index.html` le statistiche, `dati/` i due JSON che le alimentano.
  **Non si modificano a mano**: sono generati dal workspace privato
  (`02-PROVENZANO-DJ/instagram/crossover/database/`, comando `python aggiorna.py`),
  che ogni settimana ci riversa la puntata nuova
- `fonts/` — Anton e Poppins ExtraBold (OFL)
- `icons/` — icone social da [simple-icons](https://simpleicons.org) (CC0)
- `CNAME` — arriverà quando il dominio Aruba viene puntato su GitHub Pages
