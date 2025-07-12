# Strutture condizionali avanzate

Le strutture condizionali sono uno strumento fondamentale nella programmazione, che ci permette di controllare il flusso del nostro codice in base a determinate condizioni. In questo articolo approfondiremo le strutture condizionali avanzate, come if, else e switch case, per gestire in maniera più efficiente e pulita i nostri programmi.

## if

L'istruzione if è una delle più comuni e utilizzate nelle programmazione. Essa permette di eseguire un blocco di codice solo se una determinata condizione è verificata. Ad esempio:

```python
if x > 10:
    print("x è maggiore di 10")
```

In questo caso, se la variabile x è maggiore di 10, verrà stampato a schermo il messaggio "x è maggiore di 10".

## else

L'istruzione else permette di definire un blocco di codice da eseguire nel caso in cui la condizione dell'if non sia verificata. Ad esempio:

```python
if x > 10:
    print("x è maggiore di 10")
else:
    print("x è minore o uguale a 10")
```

In questo caso, se x è maggiore di 10 verrà stampato il primo messaggio, altrimenti verrà stampato il secondo.

## switch case

Lo switch case è una struttura condizionale che permette di gestire in maniera più efficiente il controllo su più casi diversi. In Python non esiste uno switch case nativo, ma possiamo simulare questo comportamento con l'utilizzo di un dizionario. Ad esempio:

```python
def switch(case):
    switcher = {
        1: "Hai scelto il caso 1",
        2: "Hai scelto il caso 2",
        3: "Hai scelto il caso 3"
    }
    
    return switcher.get(case, "Scelta non valida")

print(switch(1))
```

In questo caso, se passiamo alla funzione switch il valore 1, verrà restituito il messaggio "Hai scelto il caso 1". Se passiamo un valore diverso da 1, 2 o 3, verrà restituito il messaggio "Scelta non valida".

## Conclusioni

Le strutture condizionali avanzate come if, else e switch case ci permettono di gestire in maniera più efficace e pulita le condizioni all'interno dei nostri programmi. È importante conoscerne il funzionamento e saperle utilizzare correttamente per scrivere codice più chiaro e leggibile.