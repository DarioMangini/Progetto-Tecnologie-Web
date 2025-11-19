# TWEB-PROGETTO_Mangini-Melluso

**Progetto gruppo Dario Mangini, Raffaele Melluso**

## Descrizione

Questo progetto è una web application nata come lavoro di gruppo per il corso di Tecnologie Web (TWEB). L'applicazione presenta un portale film dal nome "Rotten Cucumber", che permette agli utenti di consultare gli ultimi film usciti, i top-rated, le nomination agli Oscar e molto altro. Include anche funzionalità di chat in tempo reale fra gli utenti.

Il backend espone anche funzionalità tramite API documentate in Swagger.

## Funzionalità principali

- Homepage con carosello dei film recenti
- Schede dettagliate dei film
- Visualizzazione dei film top-rated
- Sezione Oscar con nomination e vincitori
- Chat in tempo reale tra utenti, con stanze preimpostate (Ultime Uscite, Attori, Fun Facts, ecc.)
    - Join in una stanza tramite form (username, ruolo, scelta stanza)
    - Generazione automatica di stanze con nome casuale
- Ricerca film per titolo/nome attore/regista
- Recensioni e voti percentuali sui film
- API REST documentate via Swagger
- Navigazione reattiva e supporto dispositivi mobili (Bootstrap)
- Footer e navbar personalizzati

## Stack Tecnologico

- **Frontend:** HTML, CSS (Bootstrap), JavaScript, Handlebars
- **Backend:** Node.js, Express.js, Socket.io (per chat), MongoDB (tramite Mongoose)
- **Documentazione API:** Swagger

## Struttura del progetto

```
solution/
├── Client/
│   ├── views/
│   │   ├── index.hbs, latest.hbs, chat.hbs, partials/
│   ├── app.js
│   ├── public/
│   │   ├── javascripts/
│   │   ├── stylesheets/
│   ├── bin/www.js
├── ServerDinamicoMongo/
│   ├── app.js
│   ├── databases/
│   │   └── database.js
│   ├── routes/
│   ├── views/
│   ├── public/
│   │   └── stylesheets/
│   ├── bin/www
```

## Installazione e Avvio

1. **Prerequisiti:** Node.js, MongoDB installato e attivo sulla porta predefinita.
2. Clona il repository e installa le dipendenze:
    ```bash
    npm install
    ```
3. Avvia i server (client e backend):

    - Dalla cartella `solution/ServerDinamicoMongo/`
      ```bash
      npm start
      ```
    - Dalla cartella `solution/Client/`
      ```bash
      npm start
      ```
4. Accedi all’app da `http://localhost:3000`

## Note

- Assicurati che MongoDB sia attivo sulla porta `27017` (`mongodb://localhost:27017/DynamicData`).
- Le API sono documentate su `/api-docs` via Swagger.
- Il progetto è privato e dedicato esclusivamente a scopi didattici.

## Autori

- Dario Mangini
- Raffaele Melluso

---

Per ulteriori dettagli consulta la [documentazione Swagger](solution/Client/swagger/swaggerDocumentation.json) o i commenti presenti nel codice.
