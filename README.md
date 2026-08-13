OGD WinCaffè Booster & Optimizer

**Versione 1.0.35.0R3 — Windows 11 x64**

WinCaffè è un’applicazione desktop dedicata al controllo, alla diagnostica e
all’ottimizzazione di Windows, con particolare attenzione al gaming, alla
reattività del sistema e alla gestione delle applicazioni più pesanti.

Il progetto riunisce una moderna interfaccia grafica e il motore operativo
**OGD WinCaffè 10.0.0 Old UI**, aggiornato e corretto per questa release.

> WinCaffè interviene su impostazioni di sistema, processi, servizi e profili
> energetici. Prima di applicare modifiche importanti è sempre consigliato
> creare un punto di ripristino o un backup.

## A chi è destinato

WinCaffè è pensato per chi desidera:

- conoscere in tempo reale lo stato del proprio PC;
- preparare Windows per il gaming;
- assegnare più risorse a giochi e applicazioni selezionate;
- ridurre attività in background non necessarie;
- controllare RAM, dischi, rete e processi;
- applicare ottimizzazioni guidate senza modificare manualmente il registro;
- conservare un registro leggibile delle operazioni eseguite.

Non è necessario conoscere PowerShell. Le funzioni principali sono accessibili
dall’interfaccia; l’Ottimizzatore Avanzato utilizza invece una console guidata
con menu numerati.

## Funzioni principali

### Dashboard Live

La schermata iniziale offre una panoramica del computer:

- utilizzo in tempo reale di CPU e RAM;
- nome e classe prestazionale di CPU e GPU;
- quantità e caratteristiche della memoria;
- spazio disponibile sul disco di sistema;
- scheda di rete rilevata;
- piano energetico attivo;
- tipo di dispositivo, versione Windows e versione PowerShell;
- stato dell’Auto-Boost e risoluzione del timer;
- riavvio rapido di Esplora risorse per liberare cache e ripristinare la shell.

La classificazione hardware serve come indicazione orientativa per adattare i
profili. La R3 riconosce correttamente anche i processori Ryzen X3D recenti,
compreso il Ryzen 9850X3D.

### Ottimizzazioni Pro

Da questa sezione si apre l’**Ottimizzatore Avanzato WinCaffè 10.0.0**.

La console interattiva chiede inizialmente il tipo di PC:

1. Desktop
2. Laptop
3. Laptop Gaming

Le scelte successive permettono di accedere ai profili e agli strumenti del
motore Old UI. La console deve rimanere aperta durante l’operazione e le
risposte vanno inserite nella finestra PowerShell appena comparsa.

### Auto-Boost Engine

Auto-Boost rileva giochi e applicazioni attive e può gestire automaticamente:

- priorità del processo in primo piano;
- priorità ridotta per processi secondari selezionati;
- EcoQoS per le attività compatibili;
- profili personalizzati per giochi, applicazioni ed esclusioni;
- affinità CPU e comportamento dei processi, quando abilitati dall’utente.

Auto-Boost è disattivato all’avvio: l’utente mantiene il controllo e decide
quando attivarlo.

### Applications Booster

Applications Booster assegna un profilo dedicato a un’applicazione scelta
dall’utente. È adatto ad applicazioni generiche e supporta anche scenari con
Vortex, Node.js ed Electron.

È possibile indicare il programma, selezionare il profilo e configurare le
risorse disponibili. Alla disattivazione, WinCaffè arresta il monitoraggio e
ripristina in modo sicuro il piano energetico precedente.

### Gaming Guard

Gaming Guard comprende strumenti rivolti alle sessioni di gioco:

- rilevamento dei giochi e dei processi in primo piano;
- modalità di gioco con gestione dei servizi in background;
- diagnostica hardware e latenza in tempo reale;
- controllo dello stato e ripristino delle funzioni sospese;
- gestione di giochi, applicazioni ed esclusioni personalizzate.

Usare sempre il comando di arresto o ripristino prima di chiudere una sessione
di ottimizzazione particolarmente aggressiva.

### Monitor Hardware e RAM Watchdog

Il monitor raccoglie telemetria locale del sistema. RAM Watchdog osserva
l’utilizzo della memoria e mette a disposizione interventi manuali di pulizia,
come il trim dei working set e la pulizia profonda della memoria quando
richiesta.

La pulizia della RAM non aumenta la memoria fisica installata e non deve essere
usata continuamente: Windows gestisce normalmente la cache in autonomia.

### Storage & Dischi Pro

Questa area permette di controllare lo stato dei dischi e utilizzare strumenti
di manutenzione e diagnostica. Le operazioni disponibili possono variare in
base al tipo di unità e ai dati esposti dal sistema.

Prima di qualunque intervento sullo storage è raccomandato salvare i dati
importanti. WinCaffè non sostituisce un programma professionale di recupero o
un backup verificato.

### DNS Benchmark

Confronta le prestazioni dei server DNS disponibili per aiutare l’utente a
individuare una configurazione di rete più reattiva. I risultati dipendono
dalla connessione, dal provider, dalla posizione e dal momento del test.

### Desktop & Avvio

Raccoglie funzioni per la gestione del desktop, della shell di Windows e degli
elementi che influenzano l’avvio. Controllare sempre l’elenco proposto prima di
disabilitare qualcosa di necessario al proprio lavoro.

### Console Log

Mostra messaggi, avvisi, risultati ed errori prodotti dalle azioni eseguite
nell’app. In caso di problema, copiare l’intero blocco interessato: è molto più
utile di una semplice schermata del messaggio finale.

## Requisiti

- Windows 11 a 64 bit;
- account con privilegi amministrativi;
- **.NET Desktop Runtime 10 x64**;
- PowerShell 7 consigliato;
- Windows PowerShell 5.1 utilizzabile come compatibilità di riserva;
- spazio libero sufficiente per installazione, log e backup.

Alcune funzioni dipendono dalle caratteristiche del PC, dai driver installati e
dalle autorizzazioni offerte da Windows.

## Installazione

1. Chiudere eventuali versioni precedenti di WinCaffè.
2. Creare un backup o un punto di ripristino.
3. Avviare `WinCaffeNext_Setup_1.0.35.0R3.exe`.
4. Confermare la richiesta di amministratore.
5. Scegliere se creare il collegamento sul Desktop.
6. Al termine, avviare **OGD WinCaffè Booster**.

Il percorso predefinito è:

```text
C:\Program Files\OGD PRODUCTIONS\OGD WinCaffe Booster
```

L’applicazione usa un launcher dedicato. Non è necessario avviare manualmente
file DLL o script dalla cartella di installazione.

## Primo utilizzo consigliato

1. Aprire la Dashboard e controllare che l’hardware sia rilevato correttamente.
2. Leggere eventuali avvisi nella Console Log.
3. Creare un punto di ripristino prima dei primi tweak.
4. Provare una funzione alla volta.
5. Riavviare Windows quando indicato.
6. Verificare stabilità, temperature, audio, rete e periferiche.
7. Attivare Auto-Boost o Gaming Guard solo quando servono.

Evitare di applicare contemporaneamente più profili simili: in questo modo è
più semplice capire quale modifica ha prodotto un determinato risultato.

## Sicurezza e comportamento delle ottimizzazioni

WinCaffè può modificare temporaneamente o permanentemente:

- piani e impostazioni energetiche;
- priorità e affinità dei processi;
- servizi e attività in background;
- impostazioni di rete, gaming e latenza;
- cache, memoria e comportamento della shell;
- alcune chiavi di configurazione di Windows.

Un’ottimizzazione non garantisce automaticamente più FPS. Il risultato varia
in base a hardware, driver, giochi, temperature e configurazione iniziale.
Profili estremi possono aumentare consumi, temperatura o rumorosità.

Non interrompere il PC durante un’operazione e non chiudere forzatamente la
console mentre sta applicando o ripristinando modifiche.

## Ripristino e disinstallazione

Quando una funzione offre un comando **Stop**, **Disattiva**, **Ripristina** o
equivalente, usare prima quel comando. In caso di comportamento anomalo:

1. fermare Auto-Boost, Gaming Guard o Applications Booster;
2. ripristinare il profilo energetico precedente;
3. riavviare Windows;
4. utilizzare il punto di ripristino se il problema persiste.

Per rimuovere l’app usare **Impostazioni > App > App installate > OGD WinCaffè
Booster > Disinstalla**. La disinstallazione rimuove anche la vecchia attività
pianificata WinCaffeNext, se presente.

## Risoluzione dei problemi

### Windows chiede i privilegi amministrativi

È previsto: molte ottimizzazioni richiedono autorizzazioni elevate. Verificare
che l’installer provenga dal pacchetto ufficiale prima di confermare.

### L’app richiede .NET

Installare il **.NET Desktop Runtime 10 x64**, non soltanto una versione .NET
precedente. Dopo l’installazione riavviare Windows e aprire WinCaffè dal suo
collegamento ufficiale.

### L’Ottimizzatore Avanzato apre una nuova finestra

È il comportamento corretto. Il motore 10.0.0 usa richieste interattive: digitare
le scelte nella console PowerShell, non nel registro grafico dell’app.

### Compare un errore `Read-Host` o `NonInteractive`

La R3 aggiornata avvia l’Ottimizzatore Avanzato in modalità interattiva. Se
l’errore compare ancora, è probabilmente installato un pacchetto R3 precedente:
reinstallare usando l’ultimo setup generato e verificare il relativo checksum.

### La diagnostica mostra dati incompleti

Aggiornare la diagnostica, attendere alcuni secondi e controllare la Console
Log. Sensori, temperature e dati SMART non sono esposti allo stesso modo da
tutti i driver e dispositivi.

### Un’azione sembra bloccata

Controllare se è aperta una console in attesa di una scelta. Se non lo è,
consultare la Console Log e usare il comando di annullamento dell’azione
corrente. WinCaffè limita l’annullamento al processo avviato dall’app.

### Caratteri strani nella console o nel registro

Usare PowerShell 7 aggiornato e un font compatibile con Unicode. Il problema di
visualizzazione non implica necessariamente che l’operazione sia fallita:
controllare sempre lo stato finale e il log.

## Privacy

Le funzioni principali di diagnostica e ottimizzazione lavorano localmente sul
computer. I log possono contenere nomi di processi, percorsi, componenti
hardware e informazioni sulla configurazione: controllarli prima di condividerli
pubblicamente.

## Informazioni sulla versione 1.0.35.0R3

Questa release è basata sulla SDK stabile 1.0.34.0 e integra:

- motore ufficiale OGD WinCaffè 10.0.0 Old UI;
- Applications Booster corretto e aggiornato;
- gestione sicura dell’arresto e del piano energetico;
- fallback a Windows PowerShell 5.1;
- Auto-Boost non attivo automaticamente all’avvio;
- launcher amministrativo dedicato;
- avvio interattivo corretto dell’Ottimizzatore Avanzato;
- correzione dell’inizializzazione diagnostica sul thread grafico;
- classificazione aggiornata delle CPU Ryzen X3D recenti.

## Progetto e licenza

Ideato e sviluppato da **Luigi Sestili Spurio (OldGamerDarthy)** —
**OGD And Company Productions**.

Sito: [ogdproductions.it](https://ogdproductions.it)

Il progetto è distribuito secondo i termini della **GNU General Public License
v3.0**. Consultare il file di licenza incluso nel pacchetto per il testo
completo e le condizioni applicabili.

---

**WinCaffè aiuta a controllare e ottimizzare il sistema, ma backup, prudenza e
verifica delle modifiche restano sempre parte essenziale del processo.**
