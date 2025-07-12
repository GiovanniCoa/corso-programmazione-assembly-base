# Input/Output di base

Nel mondo della programmazione, l'input/output (I/O) è un concetto fondamentale che riguarda la comunicazione tra un programma e l'esterno. In questo articolo, ci concentreremo sull'I/O di base, ossia la lettura da tastiera e la stampa a schermo tramite interruzioni.

## Lettura da tastiera

La lettura da tastiera è un'operazione comune in molti programmi, poiché consente all'utente di interagire con il software. In linguaggi di programmazione come C o Java, è possibile leggere l'input dell'utente utilizzando funzioni apposite come `scanf` in C o `Scanner` in Java.

Ad esempio, in C è possibile leggere un intero da tastiera utilizzando il seguente codice:

```c
int numero;
scanf("%d", &numero);
```

In questo caso, `%d` specifica che si sta leggendo un intero e `&numero` indica la variabile in cui memorizzare il valore letto.

## Stampa a schermo via interruzioni

La stampa a schermo è un'altra operazione comune che permette di visualizzare dati o messaggi all'utente. In molti linguaggi di programmazione, è possibile stampare a schermo utilizzando funzioni come `printf` in C o `System.out.println` in Java.

Ad esempio, per stampare un messaggio di saluto in C si può utilizzare il seguente codice:

```c
printf("Ciao, mondo!\n");
```

In questo caso, `printf` viene utilizzata per formattare e stampare il messaggio specificato tra virgolette.

## Conclusioni

In questo articolo abbiamo esaminato l'I/O di base, ossia la lettura da tastiera e la stampa a schermo tramite interruzioni. Queste operazioni sono fondamentali per consentire all'utente di interagire con un programma e per visualizzare informazioni importanti. È importante comprendere come utilizzare correttamente le funzioni di I/O per scrivere software efficienti e user-friendly.