# Memory Game
## Gioco del memory con varie difficoltà
Questo mini progetto javascript è stato sviluppato per l'esame di Linguaggi per sviluppo lato client-side di applicazioni web per il Master in Mobile e Web Technologies.

È stato sviluppato il classico gioco del memory che prevede 4 livelli di facoltà:
- 2 X 2 
- 4 X 4 
- 6 X 6 
- 8 X 8

Il gioco è stato sviluppato per permettere di giocare a una nuova partita senza dover ricaricare la pagina.
## Installazione
Per poter utilizzare questo gioco è necessario installare [Node.js](https://nodejs.org/) e [npm](https://nodejs.org/) . È consigliabile installare l'ultima versione di questi software.
### Dipendenze
- [Node.js](https://nodejs.org/) 16.17.0 o superiore
- [npm](https://nodejs.org/) 9.2.0 o superiore
- [Webpack](https://webpack.js.org/) 5.72.0 o superiore

### Comandi per installazione
```sh
cd memory-game
npm install
```
### Comandi per l'esecuzione
Per la compilazione eseguire:
```sh
cd memory-game
webpack
```
Oppure:
```sh
cd memory-game
npm run build
```
Per la compilazione in modalità watch eseguire:
```sh
cd memory-game
webpack --watch 
```
Oppure:
```sh
cd memory-game
npm run webpack --watch 
```
Per l'esecuzione in modalità watch eseguire:
```sh
cd memory-game
webpack serve
```
Oppure:
```sh
cd memory-game
npm run webpack serve
```
## Il Gioco
Il gioco presenterà al primo avvio un menu nel quale si potrà scegliere la difficoltà

Una volta scelta la difficoltà verrà generato il campo di gioco.

Selezionando una casella, la casella verrà scoperta e verrà visualizzato il simbolo della carta. Tale carta rimarrà girata fino a quanto sul tavolo di gioco non ci siano 2 carte scoperte.

Una volta che sul tavolo ci siano 2 carte scoperte il gioco verificherà che siano uguali, nel caso in cui siano uguali le carte di gioco rimaneranno scoperte. Nel caso contrario dopo 1 secondo il gioco provvederà a coprire le carte selezionate.

Nel caso in cui si vuole resettare il gioco che è in uno stato di "gioco in corso" è possibile cliccare il tasto "Mi Arrendo". Tale tasto attiva la rivelazione di tutte le carte di gioco e dopo 2 secondi verrà chiesto se si vuole rigiocare un'altra partita.

Nel momento in cui sono state trovate tutte le carte il gioco termina dando al giocatore le statistiche della partita giocata (Numero di mosse e tempo impiegato).
