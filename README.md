# ☕ WinCaffe Next

**WinCaffe Next** è una suite gratuita e open source per Windows 10 e Windows 11, progettata per migliorare la gestione delle risorse del PC durante il gaming e l’utilizzo di applicazioni impegnative.

Il progetto nasce dall’esperienza di **OldGamerDarthy — Luigi Sestili Spurio / OGD Productions** con un obiettivo preciso: offrire ottimizzazioni comprensibili, controllabili e reversibili, evitando modifiche estreme che possano compromettere stabilità, sicurezza o compatibilità.

## 🚀 Come funziona

WinCaffe monitora in tempo reale i processi attivi e riconosce automaticamente giochi, applicazioni, launcher e servizi collegati.

Quando viene rilevato un gioco, il motore Auto-Boost può:

- assegnare una priorità CPU adatta al tipo di gioco;
- ridurre l’impatto dei processi non essenziali sotto carico;
- proteggere audio, overlay, launcher e servizi sensibili alla latenza;
- gestire in modo adattivo CPU AMD Ryzen X3D e Intel ibride;
- ottimizzare RAM, timer di sistema e piano energetico;
- ripristinare automaticamente le impostazioni originali al termine della sessione.

WinCaffe non utilizza mai la priorità `Realtime` e non applica affinità CPU rigide senza una motivazione precisa.

## 🎮 Database gaming aggiornabile

L’app include un database con profili dedicati a giochi competitivi, titoli AAA, simulatori, launcher e sistemi anti-cheat.

Il database permette di associare a ogni eseguibile:

- categoria del processo;
- priorità consigliata;
- comportamento del booster;
- protezione da modifiche inappropriate;
- eventuali indicazioni per l’affinità CPU.

I titoli competitivi riconosciuti possono utilizzare la priorità `High`, mentre per la maggior parte dei giochi viene preferita `AboveNormal`, più equilibrata e sicura.

Le configurazioni personali dell’utente hanno sempre precedenza sul database. Gli aggiornamenti online vengono controllati e installati solamente se struttura, dimensione e contenuto risultano validi.

## ⚡ Auto-Boost persistente

Le impostazioni Auto-Boost rimangono attive dopo il riavvio di Windows.

Quando la funzione viene abilitata, WinCaffe configura automaticamente il proprio avvio. Disabilitandola, l’attività collegata viene rimossa.

L’utente conserva sempre il controllo su:

- attivazione del monitoraggio;
- priorità generale dei giochi;
- riduzione dei processi in background;
- profili personalizzati;
- esclusioni;
- ottimizzazioni individuali.

## 🧠 CPU AMD Ryzen X3D e Intel ibride

WinCaffe include una gestione migliorata delle CPU moderne.

Per i Ryzen X3D:

- utilizza tutti i core sui modelli single-CCD;
- riconosce anche Ryzen 7 9850X3D;
- sui modelli dual-CCD lascia la scelta del CCD corretto a Windows Game Mode e al driver AMD 3D V-Cache;
- evita di escludere arbitrariamente metà della CPU.

Per le CPU Intel ibride, il booster tiene conto della presenza di P-Core ed E-Core, evitando maschere aggressive quando la topologia non può essere determinata con sufficiente affidabilità.

## 💾 Ottimizzazione Storage

La sezione Storage comprende strumenti dedicati a:

- unità NVMe;
- SSD SATA;
- dischi HDD;
- TRIM e ReTrim;
- diagnostica delle unità;
- analisi dei volumi;
- ottimizzazioni NTFS compatibili con Windows.

Ogni operazione mostra:

- output PowerShell completo;
- messaggi `VERBOSE`;
- fase corrente;
- barra di avanzamento in tempo reale;
- risultato finale;
- segnalazione visiva degli errori.

WinCaffe identifica separatamente unità SATA, NVMe e USB, evitando di applicare profili incompatibili al tipo di dispositivo.

## 🧰 Controllo dei componenti .NET

Lo script principale può controllare e aggiornare tramite Winget:

- .NET Runtime;
- .NET Desktop Runtime;
- ASP.NET Core Runtime;
- .NET SDK.

Se .NET non è installato, vengono proposti i componenti .NET 10 x64 necessari.

Questo controllo appartiene allo script di manutenzione e non viene imposto durante il normale avvio dell’interfaccia.

## 📊 Altre funzionalità

WinCaffe comprende inoltre:

- monitoraggio CPU, RAM, GPU e Storage;
- RAM Watchdog configurabile;
- pulizia controllata della memoria;
- gestione della shader cache;
- diagnostica hardware;
- piani energetici dedicati;
- ottimizzazione di applicazioni selezionate;
- Gaming Guard;
- gestione della precisione del timer;
- scansione delle librerie Steam, Epic Games, Riot, Ubisoft e GOG;
- terminale grafico con output in tempo reale;
- ripristino automatico delle impostazioni modificate.

## 🛡️ Sicurezza e compatibilità

WinCaffe è progettato per essere trasparente e compatibile con i sistemi di protezione dei giochi.

Il progetto:

- non contiene telemetria;
- non raccoglie dati personali;
- non include pubblicità;
- non effettua iniezioni nei processi;
- non modifica i file dei giochi;
- non utilizza driver kernel personalizzati;
- non esegue overclock;
- non altera i processi anti-cheat;
- non imposta priorità `Realtime`;
- ripristina le impostazioni temporanee al termine del boost.

Le operazioni che richiedono privilegi amministrativi vengono eseguite attraverso la normale richiesta UAC di Windows.

## 🖥️ Requisiti

- Windows 10 o Windows 11 x64;
- .NET Desktop Runtime 10;
- PowerShell 7 consigliato;
- privilegi amministrativi per le ottimizzazioni di sistema.

Per compilare il progetto sono richiesti:

- .NET 10 SDK;
- PowerShell 7;
- Inno Setup 6 per generare l’installer.

## 📦 Installazione

1. Scarica l’ultima versione dalla sezione **Releases**.
2. Avvia `WinCaffeNext_Setup_1.0.35.1.exe`.
3. Conferma la richiesta UAC.
4. Apri la sezione Auto-Boost e scegli le funzioni desiderate.
5. Usa la scansione delle librerie per aggiungere automaticamente i giochi installati.

È possibile installare una nuova versione sopra quella precedente. Le impostazioni personali dell’Auto-Boost vengono mantenute.

## 🧪 Stato della versione 1.0.35.1

La versione 1.0.35.1 introduce:

- Auto-Boost persistente;
- database gaming aggiornabile;
- 83 profili e 169 eseguibili unici;
- gestione migliorata di Ryzen X3D;
- priorità selettive per gioco;
- protezione dei processi anti-cheat;
- barra di avanzamento per le operazioni Storage;
- ripristino del controllo dei componenti .NET;
- correzione del primo avvio dopo l’installazione;
- sincronizzazione della lista giochi;
- rimozione della funzione OpenDyslexic;
- ulteriori correzioni di stabilità e sicurezza.

## 🤝 Contributi

Segnalazioni, test e proposte sono benvenuti.

Quando apri una segnalazione, indica possibilmente:

- versione di Windows;
- modello della CPU;
- quantità di RAM;
- modello della GPU;
- gioco o applicazione interessata;
- messaggi presenti nel terminale di WinCaffe;
- passaggi necessari per riprodurre il problema.

Non pubblicare password, token, nomi utente o altre informazioni personali.

## 📜 Licenza

WinCaffe Next è un progetto gratuito e open source distribuito con licenza **GNU GPL v3.0**.

Sviluppato da **OldGamerDarthy — Luigi Sestili Spurio / OGD Productions** con il contributo degli utenti, dei tester e degli strumenti di intelligenza artificiale utilizzati durante lo sviluppo.

---

☕ **WinCaffe Next — più controllo sul PC, più risorse per ciò che conta.**
