# SESTANTE — cartella di pubblicazione

Questa cartella **è il sito**. Quello che c'è qui dentro è esattamente quello
che va caricato su GitHub, senza rinominare né riorganizzare niente.

## File

- `index.html` — l'applicazione. Si chiama così perché GitHub serve
  automaticamente il file `index.html` quando qualcuno apre l'indirizzo.
  È lo stesso contenuto di Sestante 2, con in più due righe che chiedono ai
  motori di ricerca di non indicizzare la pagina.
- `robots.txt` — dice a Google e Bing di stare fuori. Obbediscono.

## Come si pubblica la prima volta

1. github.com → accedi → **+** in alto a destra → **New repository**
2. Nome breve e muto (es. `sm-t-01`), lascia **Public**, **Create repository**
3. **uploading an existing file** → trascina dentro i file di questa cartella
   → **Commit changes**
4. **Settings** → **Pages** → Source: *Deploy from a branch*, branch **main**,
   cartella **/ (root)** → **Save**
5. Dopo un minuto l'indirizzo compare in cima a quella pagina:
   `https://<nomeutente>.github.io/<nome-repository>/`

## Come si aggiorna

Apri il repository → clicca su `index.html` → l'icona della matita →
cancella tutto e incolla il nuovo contenuto → **Commit changes**.
Oppure **Add file → Upload files** e ricarica il file: sostituisce quello
vecchio. Sul telefono la versione nuova arriva alla ricarica della pagina.

## Perché siamo finiti qui — da non dimenticare

Il 12/10/2026 Chrome per Android ha **smesso di aprire gli indirizzi
`file:///`**: lo stesso file che funzionava alle 14 veniva rifiutato alle 19.
Prima ancora, aperto dai Download di Chrome, l'indirizzo era `content://`,
che per il browser è un'origine senza identità: sensore di movimento, GPS e
blocco schermo venivano negati **tutti e tre insieme**. Quella tripletta di
spie rosse è la firma del problema di origine, non di sensore.

Un indirizzo `https://` chiude la questione per sempre: contesto fidato,
sensori concessi, permesso del GPS confinato a quel dominio invece che a
tutti i file locali del telefono.

## Regola di igiene — non negoziabile

La pagina è **pubblica**. In questi file non ci va **niente** che non
metteresti su una cartolina: nessuna coordinata del terreno, nessun rilievo,
nessun dato di famiglia. L'applicazione è uno strumento di misura vuoto; i
dati stanno nel browser del telefono e non escono di lì.

Se un domani servisse metterci dentro qualcosa di davvero privato, cambia
l'ospite: GitHub Pro tiene private anche le Pages (~4 €/mese), oppure
Cloudflare Access mette un login davanti alla pagina, gratis.
