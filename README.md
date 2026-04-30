# Registro Ore

PWA (Progressive Web App) per il tracciamento delle ore lavorative giornaliere.  
Funziona direttamente nel browser, senza installazione, senza account, senza server.

## Funzionalità principali

- Inserimento giornaliero di ingresso e uscita con calcolo automatico di straordinari o ore mancanti
- Calendario mensile per navigare rapidamente tra i giorni
- Gestione assenze: Ferie, Malattia, Permesso (tutta la giornata o ore parziali)
- Archivio storico con filtri per tipo di giornata e barra di ricerca
- Festività configurabili con aggiornamento automatico al cambio anno
- Esportazione dati in formato XLSX (un foglio per mese con totali) e CSV
- Backup e ripristino completo tramite file JSON
- Reminder automatico di backup settimanale
- Funziona offline dopo il primo caricamento

## Come usarla

Apri il link nel browser del tuo telefono o computer.  
Su **Android (Chrome)**: menu ⋮ → "Aggiungi a schermata Home"  
Su **iPhone (Safari)**: tasto condividi → "Aggiungi a schermata Home"

L'app si comporta come un'applicazione nativa, senza bisogno di app store.

## Dove vengono salvati i dati

I dati vengono salvati nel **localStorage** del browser, localmente sul tuo dispositivo.  
Non vengono trasmessi a nessun server. Ogni persona che usa l'app ha il proprio archivio privato e separato.

> ⚠️ Pulire la cache del browser cancella anche i dati dell'app.  
> Si consiglia di esportare un backup periodico da **Settings → Backup**.

## Impostazioni configurabili

- Ore lavorative dovute al giorno (default: 8h)
- Pausa pranzo default (default: 60 min)
- Orario di ingresso e uscita default
- Anno di riferimento per le festività
- Festività personalizzabili (aggiungi, modifica, elimina)

## Esportazione

Da **Settings → Esportazione dati**:
- **XLSX**: un foglio Excel per ogni mese, con riga di totale finale
- **CSV**: formato universale compatibile con qualsiasi applicazione

## Backup e ripristino

Da **Settings → Backup e ripristino**:
- **Esporta backup**: scarica un file JSON con tutti i dati (giorni, festività, impostazioni)
- **Importa backup**: ripristina da un file JSON precedente con anteprima dei dati

## Tecnologie

HTML, CSS, JavaScript vanilla — nessuna dipendenza esterna, nessun framework.  
I dati vengono salvati tramite `localStorage` del browser.

## Versione

1.3
