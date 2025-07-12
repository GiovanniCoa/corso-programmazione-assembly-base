# Sintassi di base dell'Assembly

L'Assembly è un linguaggio di programmazione a basso livello che consente di comunicare direttamente con l'hardware di un computer. È caratterizzato da una sintassi particolare, che richiede una certa familiarità con i dettagli dell'architettura del processore su cui si sta lavorando.

## Struttura di un programma Assembly

Un programma scritto in Assembly è composto da una serie di istruzioni che vengono eseguite sequenzialmente dal processore. Ogni istruzione ha un'operazione da eseguire e uno o più operandi su cui agire. La struttura di base di un programma Assembly include:

- **Etichette**: sono utilizzate per identificare punti specifici nel programma e consentono di fare riferimento a tali punti in altre parti del codice. Le etichette vengono precedute dal simbolo ":" e devono essere uniche all'interno del programma.

- **Direttive**: vengono utilizzate per definire informazioni aggiuntive per il compilatore, come ad esempio l'allocazione di memoria per variabili o costanti. Le direttive sono precedute dal simbolo "@".

- **Istruzioni**: rappresentano le operazioni da eseguire dal processore. Ogni istruzione è composta da un'operazione seguita da uno o più operandi su cui agisce l'operazione. Le istruzioni possono essere di diversi tipi, come ad esempio istruzioni di movimento di dati, istruzioni aritmetiche o istruzioni di controllo del flusso.

## Esempio di programma Assembly

Di seguito viene mostrato un esempio di programma Assembly che calcola la somma di due numeri e la memorizza in una variabile:

```
@Dati
NUM1 DB 10
NUM2 DB 20
RISULTATO DB ?

@Codice
MOV AX, @Dati.NUM1
ADD AX, @Dati.NUM2
MOV @Dati.RISULTATO, AX
```

In questo esempio, le direttive @Dati definiscono tre variabili: NUM1 e NUM2 che contengono i due numeri da sommare, e RISULTATO che conterrà il risultato della somma. Le istruzioni MOV e ADD vengono utilizzate per spostare i dati tra i registri del processore e eseguire l'operazione di somma.

## Conclusione

La sintassi dell'Assembly può risultare complessa per chi non è abituato a lavorare a basso livello con l'hardware di un computer. Tuttavia, una volta compresa la struttura di base di un programma Assembly e le sue istruzioni fondamentali, è possibile scrivere codice efficiente e ottimizzato per sfruttare al meglio le potenzialità del processore.