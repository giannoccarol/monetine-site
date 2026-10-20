---
layout: default
title: "Informativa sulla privacy di Monetine"
lang: it
---

# Informativa sulla privacy di Monetine

Ultimo aggiornamento: 20 ottobre 2026

Monetine è un'app Android per tenere i conti di spese, entrate e patrimonio. La sviluppa Lorenzo Giannoccaro ("noi"). Questa pagina spiega quali dati usa l'app, dove finiscono e come controllarli.

## In breve

- I tuoi dati restano sul telefono. Monetine non ha server propri, non chiede di creare un account e non ci manda nulla.
- Non ci sono pubblicità, statistiche d'uso, analytics o strumenti di tracciamento.
- Se colleghi un provider di intelligenza artificiale, Monetine gli invia il testo che detti o scrivi e un riassunto dei tuoi conti, solo quando usi una funzione AI. Il provider lo scegli tu, con la tua chiave.
- Il riconoscimento vocale è quello di sistema di Android.
- Se il backup di Android è attivo, una copia dei dati va nel tuo account Google.

## Cosa resta sul telefono

Tutto quello che inserisci è salvato solo nella memoria dell'app sul tuo telefono:

- movimenti (importo, data, titolo, categoria, negozio, note, conto);
- conti con i loro saldi mensili, categorie, spese ricorrenti, finanziamenti e import fatti;
- impostazioni dell'app (tema, promemoria, provider e modello scelti, indirizzo dell'endpoint personalizzato, somma da tenere da parte);
- le chiavi dei provider AI, cifrate con una chiave del sistema Android (Android Keystore) che non può uscire dal telefono.

Noi non abbiamo accesso a nessuno di questi dati.

## Cosa va al provider AI e quando

Le funzioni AI sono facoltative. Finché non configuri un provider in Impostazioni → Provider e API key, Monetine non invia niente a nessuno. Puoi sempre inserire e consultare i dati a mano.

Il provider lo scegli tu tra quelli in elenco (per esempio Anthropic, OpenAI, Google Gemini, Mistral, OpenRouter) oppure indichi un tuo endpoint, come un modello sul tuo computer. Monetine si collega direttamente al provider con la tua chiave: i dati non passano da noi.

**Chat e dettatura.** Quando mandi un messaggio all'assistente, scritto o dettato, Monetine invia:

- il tuo messaggio e quelli precedenti della stessa conversazione, con le proposte dell'assistente;
- un riassunto dei dati, che serve a rispondere: categorie, conti con banca e ultimo saldo, gli ultimi 40 movimenti (data, importo, titolo, categoria, negozio, conto), i totali per categoria degli ultimi sei mesi, le spese ricorrenti, quanto puoi ancora spendere nel mese, i prezzi degli acquisti ripetuti nell'ultimo anno e i finanziamenti (nome, banca o finanziaria, importi, tassi, rate).

La prova del provider in Impostazioni invia gli stessi dati, con una frase d'esempio.

**Analisi in Statistiche.** Solo quando la chiedi, Monetine invia i totali per categoria mese per mese, le spese ricorrenti, i prezzi degli acquisti ripetuti e l'elenco delle categorie.

**Import di un estratto conto.** Se c'è un provider configurato:

- per le righe che le regole dell'app non sanno classificare, invia descrizione (fino a 140 caratteri), controparte, importo, tipo e categoria scritta nel file, per farsi suggerire categoria e titolo;
- se l'app non riconosce le colonne del file, invia le prime 20 righe (ogni cella tagliata a 40 caratteri), per capire com'è fatto. Queste righe possono contenere le intestazioni messe dalla banca, come intestatario e IBAN.

**Dati tecnici.** Come ogni collegamento a internet, il provider vede l'indirizzo IP del telefono. Monetine si presenta come "Monetine/versione (Android)". Con OpenRouter invia anche il nome dell'app, con OpenCode un codice casuale per ogni conversazione.

**Cosa ne fa il provider.** Conservazione, uso e sede dei dati dipendono dalle condizioni del provider che hai scelto, con cui hai un rapporto diretto. Alcuni provider, soprattutto con i piani gratuiti, possono conservare i messaggi o usarli per migliorare i loro modelli. Alcuni hanno sede fuori dall'Unione europea, per esempio negli Stati Uniti o in Cina. Prima di collegarne uno, leggi la sua informativa. Con un modello locale i dati restano sulla tua rete.

**Cifratura.** I provider in elenco usano connessioni cifrate (HTTPS). Per un endpoint personalizzato vale l'indirizzo che scrivi tu: con `http://` il traffico non è cifrato, quindi usalo solo nella tua rete di casa.

**Contenuti generati dall'AI.** Le risposte e le proposte dell'assistente sono generate da un modello di intelligenza artificiale e possono contenere errori. Nessuna operazione dell'assistente viene salvata senza la tua conferma, salvo che tu disattivi "Conferma prima di salvare"; eliminazioni di conti e movimenti chiedono sempre conferma.

## Riconoscimento vocale

Per dettare, Monetine usa il servizio di riconoscimento vocale di sistema di Android, cioè quello impostato sul telefono (di solito quello di Google). Monetine chiede il permesso del microfono, ma non registra né salva l'audio: riceve solo il testo riconosciuto. A seconda del telefono e delle impostazioni, il servizio di sistema può elaborare la voce sul telefono o sui server del suo fornitore, secondo le condizioni di quel fornitore.

## Backup

**Backup automatico di Android.** Monetine permette il backup di Android. Se è attivo sul telefono, Android copia i dati dell'app (il database con movimenti, conti e saldi e le impostazioni) nel tuo account Google su Google Drive, e li porta sul telefono nuovo quando trasferisci i dati. Le chiavi dei provider AI sono escluse. Il backup è gestito da Google secondo le sue condizioni e noi non vi abbiamo accesso. Puoi disattivarlo dalle impostazioni di Android, nella sezione del backup.

**Backup ed export manuali.** In Impostazioni → Importa ed esporta puoi creare un backup completo (un file JSON con tutti i dati, senza le chiavi AI) o un file CSV dei movimenti. Li salvi dove scegli tu. I file non sono cifrati: conservali con cura. Ripristinare un backup sostituisce tutti i dati presenti.

## Widget, notifiche e condivisione

- I widget sulla schermata Home mostrano importi, saldi, titoli e categorie dei movimenti, visibili a chiunque guardi il telefono. Con "Nascondi importi nei widget" (Impostazioni → Promemoria, widget e scorciatoie) gli importi diventano "•••", mentre grafici, percentuali e titoli restano.
- Il promemoria serale è spento finché non lo attivi e non mostra importi.
- "Condividi" nella card dell'inflazione personale apre il menu di condivisione di Android con un testo di percentuali e prezzi. Parte solo se lo tocchi, verso l'app che scegli.

## Permessi

- **Microfono:** per dettare. Lo chiediamo la prima volta che premi il microfono.
- **Notifiche:** solo per il promemoria serale, quando lo attivi.
- **Internet:** solo per collegarsi al provider AI che hai configurato.
- **Avvio del telefono e vibrazione:** per riprogrammare il promemoria dopo un riavvio e per il feedback aptico.

## Quanto restano i dati e come cancellarli

I dati restano sul telefono finché non li cancelli. Puoi eliminare singoli movimenti, conti e finanziamenti, annullare un import, o cancellare tutto disinstallando l'app o con "Cancella dati" nelle impostazioni di Android. Il backup su Google Drive segue le regole del backup di Android. Per i dati già inviati a un provider AI, rivolgiti al provider.

## I tuoi diritti

Il Regolamento europeo sulla protezione dei dati (GDPR) ti dà il diritto di accedere ai tuoi dati, correggerli, cancellarli, limitarne il trattamento, opporti e riceverli in un formato leggibile (portabilità). Poiché noi non conserviamo i tuoi dati, la maggior parte di questi diritti la eserciti direttamente nell'app: puoi vedere, modificare, esportare ed eliminare tutto. Per i dati inviati a un provider AI, scrivi al provider.

Per qualsiasi domanda su questa informativa scrivi a lorenzo.giannoccaro998@gmail.com. Puoi anche presentare un reclamo al Garante per la protezione dei dati personali (www.garanteprivacy.it).

## Minori

Monetine è pensata per persone maggiorenni.

## Modifiche

Se l'app cambia il modo in cui usa i dati, aggiorneremo questa pagina e la data in cima. Le modifiche importanti saranno segnalate anche nell'app.

## Contatti

Lorenzo Giannoccaro — lorenzo.giannoccaro998@gmail.com
