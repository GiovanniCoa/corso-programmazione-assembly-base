# Interruzioni e chiamate di sistema

Nel mondo della programmazione a basso livello, le interruzioni e le chiamate di sistema giocano un ruolo fondamentale nell'interfacciarsi con il sistema operativo sottostante. Le interruzioni consentono ai processi in esecuzione di comunicare con il kernel del sistema operativo, mentre le chiamate di sistema permettono l'accesso a funzionalità specifiche del sistema operativo. In questo articolo approfondiremo l'uso dell'istruzione INT per gestire le interruzioni e le chiamate di sistema.

## Le interruzioni

Le interruzioni sono segnali generati dal hardware o dal software che interrompono il normale flusso di esecuzione del programma. Le interruzioni hardware sono generate da dispositivi esterni, come tastiere o mouse, mentre le interruzioni software sono generate dal software stesso. Le interruzioni consentono ai processi di comunicare con il kernel del sistema operativo per eseguire operazioni privilegiate, come la lettura/scrittura su file, l'allocazione di memoria o la gestione dei dispositivi.

## Le chiamate di sistema

Le chiamate di sistema sono interfacce fornite dal sistema operativo per consentire ai processi utente di accedere alle funzionalità del sistema operativo. Le chiamate di sistema forniscono un modo sicuro per eseguire operazioni privilegiate senza compromettere la sicurezza del sistema. Le chiamate di sistema possono essere utilizzate per eseguire operazioni come la creazione di processi, la lettura/scrittura su file, la gestione dei dispositivi e molto altro.

## L'istruzione INT

L'istruzione INT (interrupt) è utilizzata per generare un'eccezione software, cioè un'interfaccia tra il programma utente e il kernel del sistema operativo. L'istruzione INT prende un numero di interruzione come argomento e passa il controllo al gestore dell'interfaccia corrispondente nel kernel. Ad esempio, l'istruzione INT 80h è comunemente utilizzata per eseguire chiamate di sistema in ambiente Linux.

```assembly
mov eax, 4       ; codice della chiamata di sistema per la scrittura su file
mov ebx, 1       ; file descriptor per lo standard output
mov ecx, msg     ; puntatore al messaggio da stampare
mov edx, len     ; lunghezza del messaggio
int 80h          ; esegue la chiamata di sistema
```

Nell'esempio sopra, il codice assembly esegue una chiamata di sistema per stampare un messaggio sullo standard output utilizzando l'istruzione INT 80h.

## Conclusioni

Le interruzioni e le chiamate di sistema sono elementi fondamentali per l'interfacciarsi con il sistema operativo e accedere alle funzionalità privilegiate. L'istruzione INT permette di gestire le interruzioni e le chiamate di sistema in modo efficiente e sicuro. È importante comprendere il funzionamento di queste istruzioni per sviluppare software robusto e performante.