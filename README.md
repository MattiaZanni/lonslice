# longslice 
*diario*

>**Descrizione**
 
 Data una stringa formata solo da cifre, calcolare il prodotto più grande per una sua sottostringa contigua di cifre di lunghezza N

<img height="600" width="400" src="https://user-images.githubusercontent.com/127590037/235289848-c6237a32-9b88-4c50-8e7a-a62468617864.png" />


>commento del codice

Il codice prende in input una stringa di cifre e un intero "n" che rappresenta la lunghezza della serie di cifre da moltiplicare, restituisce il prodotto più grande possibile della serie di lunghezza "n" all'interno della stringa di cifre.
La prima cosa che fa è verificare se "n" è maggiore della lunghezza della stringa di cifre.
Se è così, viene generata un'eccezione ArgumentException.
Il metodo quindi inizializza una variabile "maxProduct" a 0 e un contatore "i" a 0.
Viene poi eseguito un ciclo "while" finché "i" è minore o uguale alla lunghezza della stringa di cifre meno "n".
All'interno del ciclo "while", viene inizializzata una variabile "product" a 1 e viene eseguito un ciclo "for" per moltiplicare ogni cifra nella serie di lunghezza
"n".
Se viene trovato un carattere non numerico, il ciclo "for" viene interrotto e l'indice "i" viene spostato alla posizione successiva alla posizione non numerica trovata.
Se la moltiplicazione della serie di cifre corrente è maggiore del valore attuale di "maxProduct", "maxProduct" viene aggiornato con la moltiplicazione della serie di cifre corrente.
Infine, l'indice "i" viene incrementato di uno e il ciclo "while" continua finché tutte le serie di cifre di lunghezza "n" all'interno della stringa di cifre.
