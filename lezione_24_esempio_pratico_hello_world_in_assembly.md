# Esempio pratico: Hello World in Assembly

Nel mondo della programmazione, scrivere un semplice programma "Hello World" è spesso il primo passo per imparare un nuovo linguaggio. In questo articolo, fornirò un esempio pratico di come scrivere, compilare ed eseguire un programma "Hello World" in linguaggio Assembly.

## Passo 1: Scrivere il codice Assembly

Prima di tutto, è necessario scrivere il codice Assembly per stampare il messaggio "Hello World" a schermo. Di seguito è riportato un esempio di codice Assembly per farlo:

```assembly
section .data
    msg db 'Hello World', 0

section .text
    global _start

_start:
    ; scrivi il messaggio "Hello World" a schermo
    mov eax, 4
    mov ebx, 1
    mov ecx, msg
    mov edx, 11
    int 0x80

    ; esci dal programma
    mov eax, 1
    xor ebx, ebx
    int 0x80
```

## Passo 2: Compilare il codice Assembly

Una volta scritto il codice Assembly, è necessario compilarlo utilizzando un assembler come NASM. Ecco come si può compilare il codice Assembly "Hello World":

```bash
nasm -f elf hello.asm -o hello.o
ld hello.o -o hello
```

## Passo 3: Eseguire il programma

Dopo aver compilato il codice Assembly, è possibile eseguire il programma "Hello World" digitando il seguente comando:

```bash
./hello
```

Una volta eseguito il programma, si dovrebbe vedere il messaggio "Hello World" stampato a schermo.

In conclusione, questo articolo ha fornito un esempio pratico di come scrivere, compilare ed eseguire un programma "Hello World" in linguaggio Assembly. Questo semplice esempio può aiutare a comprendere i concetti di base della programmazione in Assembly e preparare il terreno per progetti più complessi. Spero che questo articolo sia stato utile e ti abbia ispirato a esplorare ulteriormente il linguaggio Assembly. Buon coding!