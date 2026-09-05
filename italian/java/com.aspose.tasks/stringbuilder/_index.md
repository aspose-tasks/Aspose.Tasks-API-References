---
title: "StringBuilder"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta una stringa mutabile di caratteri."
type: docs
weight: 281
url: /it/java/com.aspose.tasks/stringbuilder/
---

**Inheritance:**
java.lang.Object
```
public final class StringBuilder
```

Rappresenta una stringa mutabile di caratteri. Non può essere estesa.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [StringBuilder()](#StringBuilder--) | Inizializza una nuova istanza della classe StringBuilder. |
| [StringBuilder(int capacity)](#StringBuilder-int-) | Inizializza una nuova istanza della classe StringBuilder utilizzando la capacità specificata. |
| [StringBuilder(int capacity, int maxCapacity)](#StringBuilder-int-int-) | Inizializza una nuova istanza della classe StringBuilder che inizia con una capacità specificata e può crescere fino a un massimo specificato. |
| [StringBuilder(String value)](#StringBuilder-java.lang.String-) | Inizializza una nuova istanza della classe StringBuilder utilizzando la stringa specificata. |
| [StringBuilder(String value, int capacity)](#StringBuilder-java.lang.String-int-) | Inizializza una nuova istanza della classe StringBuilder utilizzando la stringa e la capacità specificate. |
| [StringBuilder(String value, int startIndex, int length, int capacity)](#StringBuilder-java.lang.String-int-int-int-) | Inizializza una nuova istanza della classe StringBuilder dalla sottostringa e dalla capacità specificate. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [append(boolean value)](#append-boolean-) | Aggiunge la rappresentazione stringa di un valore booleano specificato a questa istanza. |
| [append(byte value)](#append-byte-) | Aggiunge la rappresentazione stringa di un byte specificato a questa istanza. |
| [append(char value)](#append-char-) | Aggiunge la rappresentazione stringa di un carattere Unicode specificato a questa istanza. |
| [append(char value, int repeatCount)](#append-char-int-) | Aggiunge un numero specificato di copie della rappresentazione stringa di un carattere Unicode a questa istanza. |
| [append(char[] value)](#append-char---) | Aggiunge la rappresentazione stringa dei caratteri Unicode in un array specificato a questa istanza. |
| [append(char[] value, int startIndex, int charCount)](#append-char---int-int-) | Aggiunge la rappresentazione stringa di un sottoarray specificato di caratteri Unicode a questa istanza. |
| [append(double value)](#append-double-) | Aggiunge la rappresentazione stringa di un numero double specificato a questa istanza. |
| [append(float value)](#append-float-) | Aggiunge la rappresentazione stringa di un numero float specificato a questa istanza. |
| [append(int value)](#append-int-) | Aggiunge la rappresentazione stringa di un numero int specificato a questa istanza. |
| [append(Object value)](#append-java.lang.Object-) | Aggiunge la rappresentazione stringa di un oggetto specificato a questa istanza. |
| [append(String value)](#append-java.lang.String-) | Aggiunge una copia della stringa specificata a questa istanza. |
| [append(String value, int startIndex, int count)](#append-java.lang.String-int-int-) | Aggiunge una copia di una sottostringa specificata a questa istanza. |
| [append(BigDecimal value)](#append-java.math.BigDecimal-) | Aggiunge la rappresentazione stringa di un numero BigDecimal specificato a questa istanza. |
| [append(long value)](#append-long-) | Aggiunge la rappresentazione stringa di un numero long specificato a questa istanza. |
| [append(short value)](#append-short-) | Aggiunge la rappresentazione stringa di un numero short specificato a questa istanza. |
| [appendFormat(String format, Object[] args)](#appendFormat-java.lang.String-java.lang.Object...-) | Aggiunge la stringa restituita dall'elaborazione di una stringa di formato composito, che contiene zero o più elementi di formato, a questa istanza. |
| [appendLine()](#appendLine--) | Aggiunge il terminatore di riga predefinito alla fine dell'oggetto StringBuilder corrente. |
| [appendLine(String value)](#appendLine-java.lang.String-) | Aggiunge una copia della stringa specificata seguita dal terminatore di riga predefinito alla fine dell'oggetto StringBuilder corrente. |
| [copyTo(int sourceIndex, char[] destination, int destinationIndex, int count)](#copyTo-int-char---int-int-) | Copia i caratteri da un segmento specificato di questa istanza a un segmento specificato di un array Char di destinazione. |
| [ensureCapacity(int capacity)](#ensureCapacity-int-) | Garantisce che la capacità di questa istanza di StringBuilder sia almeno il valore specificato. |
| [equals(Object obj)](#equals-java.lang.Object-) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| [getCapacity()](#getCapacity--) | Ottiene il numero massimo di caratteri che può essere contenuto nella memoria allocata dall'istanza corrente. |
| [getLength()](#getLength--) | Ottiene la lunghezza dell'oggetto StringBuilder corrente. |
| [getMaxCapacity()](#getMaxCapacity--) | Ottiene la capacità massima di questa istanza. |
| [hashCode()](#hashCode--) | Restituisce un codice hash per questo StringBuilder. |
| [insert(int index, boolean value)](#insert-int-boolean-) | Inserisce la rappresentazione stringa di un valore booleano in questa istanza nella posizione di carattere specificata. |
| [insert(int index, byte value)](#insert-int-byte-) | Inserisce la rappresentazione stringa di un valore byte in questa istanza nella posizione di carattere specificata. |
| [insert(int index, char value)](#insert-int-char-) | Inserisce la rappresentazione stringa di un carattere Unicode specificato in questa istanza nella posizione di carattere specificata. |
| [insert(int index, char[] value)](#insert-int-char---) | Inserisce la rappresentazione stringa di un array specificato di caratteri Unicode in questa istanza nella posizione di carattere specificata. |
| [insert(int index, char[] value, int startIndex, int charCount)](#insert-int-char---int-int-) | Inserisce la rappresentazione stringa di un sottoarray specificato di caratteri Unicode in questa istanza nella posizione di carattere specificata. |
| [insert(int index, double value)](#insert-int-double-) | Inserisce la rappresentazione stringa di un numero double in questa istanza nella posizione di carattere specificata. |
| [insert(int index, float value)](#insert-int-float-) | Inserisce la rappresentazione stringa di un numero float in questa istanza nella posizione di carattere specificata. |
| [insert(int index, int value)](#insert-int-int-) | Inserisce la rappresentazione stringa di un numero int in questa istanza nella posizione di carattere specificata. |
| [insert(int index, Object value)](#insert-int-java.lang.Object-) | Inserisce la rappresentazione stringa di un oggetto in questa istanza nella posizione di carattere specificata. |
| [insert(int index, String value)](#insert-int-java.lang.String-) | Inserisce una stringa in questa istanza nella posizione di carattere specificata. |
| [insert(int index, String value, int count)](#insert-int-java.lang.String-int-) | Inserisce una o più copie di una stringa specificata in questa istanza nella posizione di carattere specificata. |
| [insert(int index, BigDecimal value)](#insert-int-java.math.BigDecimal-) | Inserisce la rappresentazione stringa di un numero decimale in questa istanza nella posizione di carattere specificata. |
| [insert(int index, long value)](#insert-int-long-) | Inserisce la rappresentazione stringa di un numero long in questa istanza nella posizione di carattere specificata. |
| [insert(int index, short value)](#insert-int-short-) | Inserisce la rappresentazione stringa di un numero short in questa istanza nella posizione di carattere specificata. |
| [remove(int startIndex, int length)](#remove-int-int-) | Rimuove l'intervallo specificato di caratteri da questa istanza. |
| [replace(char oldChar, char newChar)](#replace-char-char-) | Sostituisce tutte le occorrenze di un carattere specificato in questa istanza con un altro carattere specificato. |
| [replace(char oldValue, char newValue, int startIndex, int count)](#replace-char-char-int-int-) | Sostituisce, all'interno di una sottostringa di questa istanza, tutte le occorrenze di un carattere specificato con un altro carattere specificato. |
| [replace(String oldValue, String newValue)](#replace-java.lang.String-java.lang.String-) | Sostituisce tutte le occorrenze di una stringa specificata in questa istanza con un'altra stringa specificata. |
| [replace(String oldValue, String newValue, int startIndex, int count)](#replace-java.lang.String-java.lang.String-int-int-) | Sostituisce, all'interno di una sottostringa di questa istanza, tutte le occorrenze di una stringa specificata con un'altra stringa specificata. |
| [setCapacity(int value)](#setCapacity-int-) | Imposta il numero massimo di caratteri che possono essere contenuti nella memoria allocata dall'istanza corrente. |
| [setLength(int value)](#setLength-int-) | Imposta la lunghezza dell'oggetto StringBuilder corrente. |
| [toString()](#toString--) | Converte il valore di questa istanza in una stringa. |
| [toString(int startIndex, int length)](#toString-int-int-) | Converte il valore di una sottostringa di questa istanza in una stringa. |
### StringBuilder() {#StringBuilder--}
```
public StringBuilder()
```


Inizializza una nuova istanza della classe StringBuilder.

### StringBuilder(int capacity) {#StringBuilder-int-}
```
public StringBuilder(int capacity)
```


Inizializza una nuova istanza della classe StringBuilder utilizzando la capacità specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| capacità | int | La dimensione iniziale suggerita per questa istanza. |

### StringBuilder(int capacity, int maxCapacity) {#StringBuilder-int-int-}
```
public StringBuilder(int capacity, int maxCapacity)
```


Inizializza una nuova istanza della classe StringBuilder che inizia con una capacità specificata e può crescere fino a un massimo specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| capacità | int | La dimensione iniziale suggerita per lo StringBuilder. |
| capacitàMassima | int | Il numero massimo di caratteri che la stringa corrente può contenere. |

### StringBuilder(String value) {#StringBuilder-java.lang.String-}
```
public StringBuilder(String value)
```


Inizializza una nuova istanza della classe StringBuilder utilizzando la stringa specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | La stringa usata per inizializzare il valore dell'istanza. |

### StringBuilder(String value, int capacity) {#StringBuilder-java.lang.String-int-}
```
public StringBuilder(String value, int capacity)
```


Inizializza una nuova istanza della classe StringBuilder utilizzando la stringa e la capacità specificate.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | La stringa usata per inizializzare il valore dell'istanza. |
| capacità | int | La dimensione iniziale suggerita per lo StringBuilder. |

### StringBuilder(String value, int startIndex, int length, int capacity) {#StringBuilder-java.lang.String-int-int-int-}
```
public StringBuilder(String value, int startIndex, int length, int capacity)
```


Inizializza una nuova istanza della classe StringBuilder dalla sottostringa e dalla capacità specificate.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | La stringa che contiene la sottostringa usata per inizializzare il valore di questa istanza. |
| indiceInizio | int | La posizione all'interno del valore dove inizia la sottostringa. |
| lunghezza | int | Il numero di caratteri nella sottostringa. |
| capacità | int | La dimensione iniziale suggerita per lo StringBuilder. |

### append(boolean value) {#append-boolean-}
```
public StringBuilder append(boolean value)
```


Aggiunge la rappresentazione stringa di un valore booleano specificato a questa istanza.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | Il valore booleano da aggiungere. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(byte value) {#append-byte-}
```
public StringBuilder append(byte value)
```


Aggiunge la rappresentazione stringa di un byte specificato a questa istanza.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | byte | Il valore da aggiungere. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char value) {#append-char-}
```
public StringBuilder append(char value)
```


Aggiunge la rappresentazione stringa di un carattere Unicode specificato a questa istanza.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | char | Il carattere Unicode da aggiungere. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char value, int repeatCount) {#append-char-int-}
```
public StringBuilder append(char value, int repeatCount)
```


Aggiunge un numero specificato di copie della rappresentazione stringa di un carattere Unicode a questa istanza.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | char | Il carattere da aggiungere. |
| repeatCount | int | Il numero di volte per aggiungere il valore. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char[] value) {#append-char---}
```
public StringBuilder append(char[] value)
```


Aggiunge la rappresentazione stringa dei caratteri Unicode in un array specificato a questa istanza.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | char[] | L'array di caratteri da aggiungere. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char[] value, int startIndex, int charCount) {#append-char---int-int-}
```
public StringBuilder append(char[] value, int startIndex, int charCount)
```


Aggiunge la rappresentazione stringa di un sottoarray specificato di caratteri Unicode a questa istanza.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | char[] | Un array di caratteri. |
| indiceInizio | int | La posizione iniziale nel valore. |
| charCount | int | Il numero di caratteri da aggiungere. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(double value) {#append-double-}
```
public StringBuilder append(double value)
```


Aggiunge la rappresentazione stringa di un numero double specificato a questa istanza.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double | Il valore da aggiungere. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(float value) {#append-float-}
```
public StringBuilder append(float value)
```


Aggiunge la rappresentazione stringa di un numero float specificato a questa istanza.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | float | Il valore da aggiungere. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(int value) {#append-int-}
```
public StringBuilder append(int value)
```


Aggiunge la rappresentazione stringa di un numero int specificato a questa istanza.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | Il valore da aggiungere. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(Object value) {#append-java.lang.Object-}
```
public StringBuilder append(Object value)
```


Aggiunge la rappresentazione stringa di un oggetto specificato a questa istanza.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.Object | L'oggetto da aggiungere. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(String value) {#append-java.lang.String-}
```
public StringBuilder append(String value)
```


Aggiunge una copia della stringa specificata a questa istanza.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | La stringa da aggiungere. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(String value, int startIndex, int count) {#append-java.lang.String-int-int-}
```
public StringBuilder append(String value, int startIndex, int count)
```


Aggiunge una copia di una sottostringa specificata a questa istanza.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | La stringa che contiene la sottostringa da aggiungere. |
| indiceInizio | int | La posizione iniziale della sottostringa all'interno del valore. |
| count | int | Il numero di caratteri nel valore da aggiungere. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(BigDecimal value) {#append-java.math.BigDecimal-}
```
public StringBuilder append(BigDecimal value)
```


Aggiunge la rappresentazione stringa di un numero BigDecimal specificato a questa istanza.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.math.BigDecimal | Il valore da aggiungere. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(long value) {#append-long-}
```
public StringBuilder append(long value)
```


Aggiunge la rappresentazione stringa di un numero long specificato a questa istanza.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | long | Il valore da aggiungere. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(short value) {#append-short-}
```
public StringBuilder append(short value)
```


Aggiunge la rappresentazione stringa di un numero short specificato a questa istanza.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | short | Il valore da aggiungere. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### appendFormat(String format, Object[] args) {#appendFormat-java.lang.String-java.lang.Object...-}
```
public StringBuilder appendFormat(String format, Object[] args)
```


Aggiunge la stringa restituita dall'elaborazione di una stringa di formato composito, che contiene zero o più elementi di formato, a questa istanza. Ogni elemento di formato è sostituito dalla rappresentazione stringa di un argomento corrispondente in un array di parametri.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| format | java.lang.String | Una stringa di formato composito. |
| args | java.lang.Object[] | Un array di oggetti da formattare. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with format appended. Each format item in format is replaced by the string representation of the corresponding object argument.
### appendLine() {#appendLine--}
```
public StringBuilder appendLine()
```


Aggiunge il terminatore di riga predefinito alla fine dell'oggetto StringBuilder corrente.

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### appendLine(String value) {#appendLine-java.lang.String-}
```
public StringBuilder appendLine(String value)
```


Aggiunge una copia della stringa specificata seguita dal terminatore di riga predefinito alla fine dell'oggetto StringBuilder corrente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | La stringa da aggiungere. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### copyTo(int sourceIndex, char[] destination, int destinationIndex, int count) {#copyTo-int-char---int-int-}
```
public void copyTo(int sourceIndex, char[] destination, int destinationIndex, int count)
```


Copia i caratteri da un segmento specificato di questa istanza a un segmento specificato di un array Char di destinazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceIndex | int | La posizione iniziale in questa istanza da cui verranno copiati i caratteri. L'indice è basato su zero. |
| destinazione | char[] | L'array in cui i caratteri saranno copiati. |
| destinationIndex | int | La posizione iniziale in destinazione dove i caratteri saranno copiati. L'indice è basato su zero. |
| count | int | Il numero di caratteri da copiare. |

### ensureCapacity(int capacity) {#ensureCapacity-int-}
```
public int ensureCapacity(int capacity)
```


Garantisce che la capacità di questa istanza di StringBuilder sia almeno il valore specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| capacità | int | La capacità minima da garantire. |

**Returns:**
int - La nuova capacità di questa istanza.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | java.lang.Object | Un oggetto da confrontare con questa istanza, o null. |

**Returns:**
boolean - true se questa istanza e sb hanno valori uguali per stringa, Capacity e MaxCapacity; altrimenti, false.
### getCapacity() {#getCapacity--}
```
public int getCapacity()
```


Ottiene il numero massimo di caratteri che può essere contenuto nella memoria allocata dall'istanza corrente.

**Returns:**
int - Il numero massimo di caratteri che può essere contenuto nella memoria allocata da questa istanza.
### getLength() {#getLength--}
```
public int getLength()
```


Ottiene la lunghezza dell'oggetto StringBuilder corrente.

**Returns:**
int - La lunghezza di questa istanza.
### getMaxCapacity() {#getMaxCapacity--}
```
public int getMaxCapacity()
```


Ottiene la capacità massima di questa istanza.

**Returns:**
int - Il numero massimo di caratteri che questa istanza può contenere.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Restituisce un codice hash per questo StringBuilder.

**Returns:**
int - Restituisce un valore di codice hash per questo oggetto.
### insert(int index, boolean value) {#insert-int-boolean-}
```
public StringBuilder insert(int index, boolean value)
```


Inserisce la rappresentazione stringa di un valore booleano in questa istanza nella posizione di carattere specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | La posizione in questa istanza dove inizia l'inserimento. |
| valore | boolean | Il valore da inserire. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, byte value) {#insert-int-byte-}
```
public StringBuilder insert(int index, byte value)
```


Inserisce la rappresentazione stringa di un valore byte in questa istanza nella posizione di carattere specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | La posizione in questa istanza dove inizia l'inserimento. |
| valore | byte | Il valore da inserire. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char value) {#insert-int-char-}
```
public StringBuilder insert(int index, char value)
```


Inserisce la rappresentazione stringa di un carattere Unicode specificato in questa istanza nella posizione di carattere specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | La posizione in questa istanza dove inizia l'inserimento. |
| valore | char | Il valore da inserire. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char[] value) {#insert-int-char---}
```
public StringBuilder insert(int index, char[] value)
```


Inserisce la rappresentazione stringa di un array specificato di caratteri Unicode in questa istanza nella posizione di carattere specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | La posizione in questa istanza dove inizia l'inserimento. |
| valore | char[] | L'array di caratteri da inserire. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char[] value, int startIndex, int charCount) {#insert-int-char---int-int-}
```
public StringBuilder insert(int index, char[] value, int startIndex, int charCount)
```


Inserisce la rappresentazione stringa di un sottoarray specificato di caratteri Unicode in questa istanza nella posizione di carattere specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | La posizione in questa istanza dove inizia l'inserimento. |
| valore | char[] | Un array di caratteri. |
| indiceInizio | int | L'indice iniziale all'interno del valore. |
| charCount | int | Il numero di caratteri da inserire. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, double value) {#insert-int-double-}
```
public StringBuilder insert(int index, double value)
```


Inserisce la rappresentazione stringa di un numero double in questa istanza nella posizione di carattere specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | La posizione in questa istanza dove inizia l'inserimento. |
| valore | double | Il valore da inserire. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, float value) {#insert-int-float-}
```
public StringBuilder insert(int index, float value)
```


Inserisce la rappresentazione stringa di un numero float in questa istanza nella posizione di carattere specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | La posizione in questa istanza dove inizia l'inserimento. |
| valore | float | Il valore da inserire. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, int value) {#insert-int-int-}
```
public StringBuilder insert(int index, int value)
```


Inserisce la rappresentazione stringa di un numero int in questa istanza nella posizione di carattere specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | La posizione in questa istanza dove inizia l'inserimento. |
| valore | int | Il valore da inserire. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, Object value) {#insert-int-java.lang.Object-}
```
public StringBuilder insert(int index, Object value)
```


Inserisce la rappresentazione stringa di un oggetto in questa istanza nella posizione di carattere specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | La posizione in questa istanza dove inizia l'inserimento. |
| valore | java.lang.Object | L'oggetto da inserire, o null. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, String value) {#insert-int-java.lang.String-}
```
public StringBuilder insert(int index, String value)
```


Inserisce una stringa in questa istanza nella posizione di carattere specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | La posizione in questa istanza dove inizia l'inserimento. |
| valore | java.lang.String | La stringa da inserire. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, String value, int count) {#insert-int-java.lang.String-int-}
```
public StringBuilder insert(int index, String value, int count)
```


Inserisce una o più copie di una stringa specificata in questa istanza nella posizione di carattere specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | La posizione in questa istanza dove inizia l'inserimento. |
| valore | java.lang.String | La stringa da inserire. |
| count | int | Il numero di volte per inserire il valore. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after insertion has completed.
### insert(int index, BigDecimal value) {#insert-int-java.math.BigDecimal-}
```
public StringBuilder insert(int index, BigDecimal value)
```


Inserisce la rappresentazione stringa di un numero decimale in questa istanza nella posizione di carattere specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | La posizione in questa istanza dove inizia l'inserimento. |
| valore | java.math.BigDecimal | Il valore da inserire. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, long value) {#insert-int-long-}
```
public StringBuilder insert(int index, long value)
```


Inserisce la rappresentazione stringa di un numero long in questa istanza nella posizione di carattere specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | La posizione in questa istanza dove inizia l'inserimento. |
| valore | long | Il valore da inserire. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, short value) {#insert-int-short-}
```
public StringBuilder insert(int index, short value)
```


Inserisce la rappresentazione stringa di un numero short in questa istanza nella posizione di carattere specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | La posizione in questa istanza dove inizia l'inserimento. |
| valore | short | Il valore da inserire. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### remove(int startIndex, int length) {#remove-int-int-}
```
public StringBuilder remove(int startIndex, int length)
```


Rimuove l'intervallo specificato di caratteri da questa istanza.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indiceInizio | int | La posizione basata su zero in questa istanza dove inizia la rimozione. |
| lunghezza | int | Il numero di caratteri da rimuovere. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the remove operation has completed.
### replace(char oldChar, char newChar) {#replace-char-char-}
```
public StringBuilder replace(char oldChar, char newChar)
```


Sostituisce tutte le occorrenze di un carattere specificato in questa istanza con un altro carattere specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| oldChar | char | Il carattere da sostituire. |
| newChar | char | Il carattere che sostituisce oldChar. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with oldChar replaced by newChar.
### replace(char oldValue, char newValue, int startIndex, int count) {#replace-char-char-int-int-}
```
public StringBuilder replace(char oldValue, char newValue, int startIndex, int count)
```


Sostituisce, all'interno di una sottostringa di questa istanza, tutte le occorrenze di un carattere specificato con un altro carattere specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| oldValue | char | Il carattere da sostituire. |
| newValue | char | Il carattere che sostituisce oldChar. |
| indiceInizio | int | La posizione in questa istanza in cui inizia la sottostringa. |
| count | int | La lunghezza della sottostringa. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with oldChar replaced by newChar in the range from startIndex to startIndex + count -1.
### replace(String oldValue, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public StringBuilder replace(String oldValue, String newValue)
```


Sostituisce tutte le occorrenze di una stringa specificata in questa istanza con un'altra stringa specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| oldValue | java.lang.String | La stringa da sostituire. |
| newValue | java.lang.String | La stringa che sostituisce oldValue, o null. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with all instances of oldValue replaced by newValue.
### replace(String oldValue, String newValue, int startIndex, int count) {#replace-java.lang.String-java.lang.String-int-int-}
```
public StringBuilder replace(String oldValue, String newValue, int startIndex, int count)
```


Sostituisce, all'interno di una sottostringa di questa istanza, tutte le occorrenze di una stringa specificata con un'altra stringa specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| oldValue | java.lang.String | La stringa da sostituire. |
| newValue | java.lang.String | La stringa che sostituisce oldValue, o null. |
| indiceInizio | int | La posizione in questa istanza in cui inizia la sottostringa. |
| count | int | La lunghezza della sottostringa. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with all instances of oldValue replaced by newValue in the range from startIndex to startIndex + count - 1.
### setCapacity(int value) {#setCapacity-int-}
```
public void setCapacity(int value)
```


Imposta il numero massimo di caratteri che possono essere contenuti nella memoria allocata dall'istanza corrente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | Il numero massimo di caratteri che può essere contenuto nella memoria allocata dall'istanza corrente. |

### setLength(int value) {#setLength-int-}
```
public void setLength(int value)
```


Imposta la lunghezza dell'oggetto StringBuilder corrente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | La lunghezza di questa istanza. |

### toString() {#toString--}
```
public String toString()
```


Converte il valore di questa istanza in una stringa.

**Returns:**
java.lang.String - Una stringa il cui valore è lo stesso di questa istanza.
### toString(int startIndex, int length) {#toString-int-int-}
```
public String toString(int startIndex, int length)
```


Converte il valore di una sottostringa di questa istanza in una stringa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indiceInizio | int | La posizione iniziale della sottostringa in questa istanza. |
| lunghezza | int | La lunghezza della sottostringa. |

**Returns:**
java.lang.String - Una stringa il cui valore è lo stesso della sottostringa specificata di questa istanza.
