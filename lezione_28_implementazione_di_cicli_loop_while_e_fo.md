# Implementazione di cicli: loop, while e for

Il controllo iterativo è un concetto fondamentale nella programmazione, che consente di eseguire ripetutamente un blocco di istruzioni fino a quando determinate condizioni sono soddisfatte. In Assembly, linguaggio di basso livello utilizzato per scrivere programmi direttamente in linguaggio macchina, è possibile implementare cicli utilizzando diverse strutture, tra cui i cicli `loop`, `while` e `for`.

## Ciclo loop

Il ciclo `loop` è una struttura iterativa semplice che consente di eseguire un blocco di istruzioni un numero prefissato di volte. In Assembly, il ciclo `loop` è implementato utilizzando il registro `CX` come contatore di iterazioni. Ad ogni iterazione, il contatore viene decrementato e il controllo passa al blocco di istruzioni finché il contatore non raggiunge il valore zero.

```
MOV CX, 5    ; Imposta il contatore a 5
LOOP start   ; Esegue il blocco di istruzioni fino a che CX non è zero
```

## Ciclo while

Il ciclo `while` è una struttura iterativa che consente di eseguire un blocco di istruzioni finché una determinata condizione è vera. In Assembly, il ciclo `while` può essere implementato utilizzando il comando `JNZ` (Jump if Not Zero) per controllare la condizione e il comando `JMP` (Jump) per tornare all'inizio del ciclo.

```
MOV CX, 5      ; Imposta il contatore a 5
WHILE:
    CMP CX, 0   ; Confronta CX con zero
    JNZ start   ; Salta a start se CX non è zero
```

## Ciclo for

Il ciclo `for` è una struttura iterativa che consente di eseguire un blocco di istruzioni per un numero specifico di volte. In Assembly, il ciclo `for` può essere implementato utilizzando un contatore e il comando `JMP` per controllare la condizione e il comando `INC` per incrementare il contatore.

```
MOV CX, 0      ; Imposta il contatore a 0
FOR:
    CMP CX, 5   ; Confronta CX con 5
    JGE end     ; Salta a end se CX è maggiore o uguale a 5
    ; Blocco di istruzioni
    INC CX      ; Incrementa il contatore
    JMP FOR     ; Torna all'inizio del ciclo
```

In conclusione, l'implementazione di cicli in Assembly richiede una buona comprensione dei comandi di controllo del flusso e dei registri per gestire correttamente le iterazioni. Utilizzando le strutture `loop`, `while` e `for`, è possibile scrivere codice efficiente e ben strutturato che esegue ripetutamente un blocco di istruzioni in base a determinate condizioni.