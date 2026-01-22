---
title: Come ho realizzato questo sito web
categories: ["code"] 
tags: ["sito", "portfolio", "hugo"]
params.dateFormat: ["13 Novembre 2025"]
date: 2025-11-15
---  
## Introduzione   
Ho costruito questo spazio usando Hugo, per condividere i miei progetti, esperimenti e qualsiasi cosa interessante su cui sto lavorando, dalla musica e sound design all'elettronica, coding e idee casuali.   
Prima di ogni altra cosa: se vuoi configurare un sito web correttamente con Hugo e il tema Blowfish, consiglio vivamente di leggere la documentazione ufficiale. È chiara, completa e molto più dettagliata di qualsiasi cosa potrei coprire qui.
Questo post è solo un breve riassunto "dietro le quinte" di come ho costruito il mio setup — niente di troppo profondo o tecnico, solo i passaggi che ho seguito e le cose che ho trovato utili mentre assemblavo il sito.   

## Pagine Ufficiali
-[Sito Ufficiale Hugo](https://gohugo.io/)
-[Sito Ufficiale Blowfish](https://blowfish.page/)
   
## Di cosa avevo bisogno   
Prima di iniziare questo sito web, dovevo avere chiaro che tipo di posto volevo costruire. Non volevo solo un blog a caso — avevo bisogno di qualcosa che si adattasse al mio modo di lavorare e al tipo di progetti che creo. In sostanza, uno spazio dove poter buttare tutto ciò su cui sto lavorando senza pensarci troppo.   
Ecco cosa sapevo di aver bisogno:   
- **Un posto per pubblicare tutti i miei progetti** — roba di produzione musicale, esperimenti di sound design, patch Max/MSP, costruzioni Arduino/ESP32, idee di stampa 3D, setup home-lab e qualsiasi altra cosa con cui sto smanettando.   
- **Facile da aggiornare** — non volevo un sistema che mi rallentasse. Scrivi un post, salvalo, fatto.   
- **Una struttura pulita** che tenga le cose organizzate senza costringermi in un flusso di lavoro complicato.   
- **Un formato che posso controllare con version control** — perché poter tracciare le modifiche (o annullare i miei errori) è sempre una salvezza.   
- **Uno strumento che mi permetta di personalizzare le cose liberamente** se un giorno decido di cambiare il design, aggiungere sezioni o ritoccare il layout.   
   
Hugo ha praticamente soddisfatto tutti questi requisiti fin da subito.   
   
## Perché ho scelto Hugo (e il tema Blowfish)   
Una volta capito di che tipo di sito web avevo bisogno, scegliere gli strumenti è diventato molto più semplice. Volevo qualcosa di veloce, leggero e flessibile — e **Hugo** mi è sembrato subito la scelta giusta. Non ha bisogno di un database, costruisce le pagine in un secondo e tutto rimane in semplici file che posso modificare quando voglio.   
Per il tema, ho scelto **Blowfish**.   
L'ho scelto principalmente perché la documentazione ufficiale è super chiara, ben organizzata e davvero facile da seguire — il che non è sempre il caso con i temi. Tutto è spiegato passo dopo passo, e ha reso l'intero processo di configurazione fluido invece che frustrante. Inoltre, il tema ha un aspetto pulito, moderno e abbastanza personalizzabile per quello che voglio costruire qui.   
Quindi sì, Hugo + Blowfish mi è sembrata la combinazione perfetta per iniziare questo sito web senza perdermi in mille impostazioni.   
   
## Come ho impostato tutto   
Configurare il sito web è stato in realtà molto più facile di quanto mi aspettassi. Hugo è super veloce da installare e una volta capita la struttura di base delle cartelle, tutto quadra. Ecco come ho impostato tutto passo dopo passo.   
### 1. Installare Hugo e Blowfish   
La prima cosa che ho fatto è stata installare la **versione Extended** di Hugo, dato che Blowfish ne ha bisogno per SCSS e altre funzionalità avanzate.   
L'ho installato usando Winget:   
```
winget install Hugo.Hugo.Extended

```
Poi ho creato un nuovo sito Hugo usando:   
```
hugo new site my-website

```
Questo ti dà istantaneamente la struttura delle cartelle:   
```
my-site/
├── archetypes/
├── assets/
├── content/
├── data/
├── i18n/
├── layouts/
├── static/
├── themes/
└── hugo.toml
```
Successivamente, ho aggiunto il tema **Blowfish** usando Git, seguendo la documentazione ufficiale:   
```
git init
git submodule add -b main https://github.com/nunocoracao/blowfish.git themes/blowfish
```
Una cosa che mi è piaciuta di Blowfish fin dall'inizio è quanto bene sono scritti i documenti — tutto è chiaro, organizzato e facile da seguire, il che ha reso la personalizzazione super fluida.   
Una volta installato il tema, sono passato a personalizzarlo. Blowfish è dotato di diversi schemi di colori integrati e ho deciso di usare la palette **Forest**.   
### 2. Creare il mio primo post   
Una volta che il sito web funzionava senza intoppi, era ora di aggiungere effettivamente dei contenuti. In Hugo, tutte le pagine e i post vivono all'interno della cartella `content`, quindi è lì che tutto deve essere posizionato. Dato che volevo una struttura pulita per gli articoli futuri, ho creato una nuova cartella chiamata `posts` all'interno di `content` — è qui che andranno tutti i miei post del blog.   
Per scrivere, non ho usato un editor di codice all'inizio. Uso già [Anytype](https://anytype.io/) ogni giorno per appunti e progetti personali, quindi mi è sembrato naturale scrivere il testo per il mio primo articolo lì. Dopo aver finito la bozza, ho semplicemente esportato il documento come file Markdown e l'ho rilasciato direttamente nella cartella `posts` che avevo creato nel progetto Hugo.   
   
