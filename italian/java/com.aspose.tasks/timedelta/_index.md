---
title: "TimeDelta"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta una differenza tra due timestamp."
type: docs
weight: 317
url: /it/java/com.aspose.tasks/timedelta/
---

**Inheritance:**
java.lang.Object
```
public class TimeDelta
```

Rappresenta una differenza tra due timestamp.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [TimeDelta(int hours, int minutes, int seconds)](#TimeDelta-int-int-int-) | Inizializza una nuova istanza di TimeDelta con il numero specificato di ore, minuti e secondi. |
| [TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds)](#TimeDelta-int-int-int-int-int-) | Inizializza una nuova istanza di TimeDelta con il numero specificato di giorni, ore, minuti, secondi e millisecondi. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add(TimeDelta other)](#add-com.aspose.tasks.TimeDelta-) | Restituisce un nuovo oggetto TimeDelta il cui valore è la somma di questa e dell'altra istanza. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [compare(TimeDelta t1, TimeDelta t2)](#compare-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-) | Confronta due valori TimeDelta e restituisce un intero che indica se il primo valore è più corto, uguale o più lungo del secondo valore. |
| [compareTo(TimeDelta other)](#compareTo-com.aspose.tasks.TimeDelta-) | Confronta questa istanza con un oggetto TimeDelta specificato e restituisce un intero che indica se questa istanza è più corta, uguale o più lunga dell'oggetto TimeSpan. |
| [equals(TimeDelta other)](#equals-com.aspose.tasks.TimeDelta-) | Indica se qualche intervallo di tempo `other` è uguale a questo. |
| [equals(TimeDelta t1, TimeDelta t2)](#equals-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-) | Verifica due istanze per l'uguaglianza. |
| [equals(Object other)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [fromDays(double value)](#fromDays-double-) | Restituisce un TimeDelta che rappresenta un numero specificato di giorni (arrotondato al millisecondo più vicino). |
| [fromHours(double value)](#fromHours-double-) | Restituisce un TimeDelta che rappresenta un numero specificato di ore (arrotondato al millisecondo più vicino). |
| [fromMilliseconds(double value)](#fromMilliseconds-double-) | Restituisce un TimeDelta che rappresenta un numero specificato di millisecondi (arrotondato al millisecondo più vicino). |
| [fromMinutes(double value)](#fromMinutes-double-) | Restituisce un TimeDelta che rappresenta un numero specificato di minuti (arrotondato al millisecondo più vicino). |
| [fromSeconds(double value)](#fromSeconds-double-) | Restituisce un TimeDelta che rappresenta un numero specificato di secondi (arrotondato al millisecondo più vicino). |
| [getDays()](#getDays--) | Restituisce la componente giorni dell'intervallo di tempo, rappresentata da questa istanza. |
| [getHours()](#getHours--) | Restituisce la componente ore dell'intervallo di tempo, rappresentata da questa istanza. |
| [getMilliseconds()](#getMilliseconds--) | Restituisce la componente millisecondi dell'intervallo di tempo, rappresentata da questa istanza. |
| [getMinutes()](#getMinutes--) | Restituisce la componente minuti dell'intervallo di tempo, rappresentata da questa istanza. |
| [getSeconds()](#getSeconds--) | Restituisce la componente secondi dell'intervallo di tempo, rappresentata da questa istanza. |
| [getTotalDays()](#getTotalDays--) | Restituisce il valore dell'istanza corrente espresso in giorni interi e frazionari. |
| [getTotalHours()](#getTotalHours--) | Restituisce il valore dell'istanza corrente espresso in ore intere e frazionarie. |
| [getTotalMilliseconds()](#getTotalMilliseconds--) | Restituisce il valore dell'istanza corrente espresso in millisecondi interi e frazionari. |
| [getTotalMinutes()](#getTotalMinutes--) | Restituisce il valore dell'istanza corrente espresso in minuti interi e frazionari. |
| [getTotalSeconds()](#getTotalSeconds--) | Restituisce il valore dell'istanza corrente espresso in secondi interi e frazionari. |
| [hashCode()](#hashCode--) | \{@inheritDoc\} |
| [negate()](#negate--) | Restituisce un nuovo `TimeDelta` il cui valore è il valore negato di questa istanza. |
| [parse(String s)](#parse-java.lang.String-) | Converte la rappresentazione stringa di un intervallo di tempo nel suo equivalente `TimeDelta`. |
| [subtract(TimeDelta other)](#subtract-com.aspose.tasks.TimeDelta-) | Restituisce un nuovo oggetto TimeDelta il cui valore è la differenza tra questa e le istanze `other`. |
| [toString()](#toString--) | \{@inheritDoc\} |
| [tryParse(String s, TimeDelta[] result)](#tryParse-java.lang.String-com.aspose.tasks.TimeDelta---) | Converte la rappresentazione stringa di un intervallo di tempo nel suo equivalente TimeDelta e restituisce un valore che indica se la conversione è riuscita. |
### TimeDelta(int hours, int minutes, int seconds) {#TimeDelta-int-int-int-}
```
public TimeDelta(int hours, int minutes, int seconds)
```


Inizializza una nuova istanza di TimeDelta con il numero specificato di ore, minuti e secondi.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ore | int | numero di ore. |
| minuti | int | numero di minuti. |
| secondi | int | numero di secondi. |

### TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds) {#TimeDelta-int-int-int-int-int-}
```
public TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds)
```


Inizializza una nuova istanza di TimeDelta con il numero specificato di giorni, ore, minuti, secondi e millisecondi.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| giorni | int | numero di giorni. |
| ore | int | numero di ore. |
| minuti | int | numero di minuti. |
| secondi | int | numero di secondi. |
| millisecondi | int | numero di millisecondi. |

### add(TimeDelta other) {#add-com.aspose.tasks.TimeDelta-}
```
public TimeDelta add(TimeDelta other)
```


Restituisce un nuovo oggetto TimeDelta il cui valore è la somma di questa e dell'altra istanza.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | l'istanza con cui sommare. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - a new object that represents the value of this instance plus value of other instance.
### clone() {#clone--}
```
public Object clone()
```




**Returns:**
java.lang.Object - \{@inheritDoc\}
### compare(TimeDelta t1, TimeDelta t2) {#compare-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-}
```
public static int compare(TimeDelta t1, TimeDelta t2)
```


Confronta due valori TimeDelta e restituisce un intero che indica se il primo valore è più corto, uguale o più lungo del secondo valore.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| t1 | [TimeDelta](../../com.aspose.tasks/timedelta) | il primo intervallo di tempo da confrontare. |
| t2 | [TimeDelta](../../com.aspose.tasks/timedelta) | il secondo intervallo di tempo da confrontare. |

**Returns:**
int - \-1 se `t1` è più corto di `t2`, 0 se `t1` è uguale a `t2` e 1 se `t1` è più lungo di `t2`.
### compareTo(TimeDelta other) {#compareTo-com.aspose.tasks.TimeDelta-}
```
public int compareTo(TimeDelta other)
```


Confronta questa istanza con un oggetto TimeDelta specificato e restituisce un intero che indica se questa istanza è più corta, uguale o più lunga dell'oggetto TimeSpan.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | un'istanza con cui confrontare. |

**Returns:**
int - \-1 se questa istanza è più corta di `other`, 0 se questa istanza è uguale a `other` e 1 se questa istanza è più lunga di `other`.
### equals(TimeDelta other) {#equals-com.aspose.tasks.TimeDelta-}
```
public boolean equals(TimeDelta other)
```


Indica se qualche intervallo di tempo `other` è uguale a questo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | intervallo di tempo con cui confrontare. |

**Returns:**
boolean - `true` se gli intervalli sono uguali; `false` altrimenti.
### equals(TimeDelta t1, TimeDelta t2) {#equals-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-}
```
public static boolean equals(TimeDelta t1, TimeDelta t2)
```


Verifica due istanze per l'uguaglianza.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| t1 | [TimeDelta](../../com.aspose.tasks/timedelta) | prima istanza. |
| t2 | [TimeDelta](../../com.aspose.tasks/timedelta) | seconda istanza. |

**Returns:**
boolean - `true` se le istanze sono uguali; `false` altrimenti.
### equals(Object other) {#equals-java.lang.Object-}
```
public boolean equals(Object other)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| altro | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### fromDays(double value) {#fromDays-double-}
```
public static TimeDelta fromDays(double value)
```


Restituisce un TimeDelta che rappresenta un numero specificato di giorni (arrotondato al millisecondo più vicino).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double | un numero di giorni. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromHours(double value) {#fromHours-double-}
```
public static TimeDelta fromHours(double value)
```


Restituisce un TimeDelta che rappresenta un numero specificato di ore (arrotondato al millisecondo più vicino).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double | un numero di ore. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromMilliseconds(double value) {#fromMilliseconds-double-}
```
public static TimeDelta fromMilliseconds(double value)
```


Restituisce un TimeDelta che rappresenta un numero specificato di millisecondi (arrotondato al millisecondo più vicino).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double | un numero di millisecondi. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromMinutes(double value) {#fromMinutes-double-}
```
public static TimeDelta fromMinutes(double value)
```


Restituisce un TimeDelta che rappresenta un numero specificato di minuti (arrotondato al millisecondo più vicino).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double | un numero di minuti. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromSeconds(double value) {#fromSeconds-double-}
```
public static TimeDelta fromSeconds(double value)
```


Restituisce un TimeDelta che rappresenta un numero specificato di secondi (arrotondato al millisecondo più vicino).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double | un numero di secondi. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### getDays() {#getDays--}
```
public int getDays()
```


Restituisce la componente giorni dell'intervallo di tempo, rappresentata da questa istanza.

**Returns:**
int - la componente giorni dell'intervallo di tempo. Può essere positivo o negativo.
### getHours() {#getHours--}
```
public int getHours()
```


Restituisce la componente ore dell'intervallo di tempo, rappresentata da questa istanza.

**Returns:**
int - la componente ore dell'intervallo di tempo nell'intervallo da -23 a 23.
### getMilliseconds() {#getMilliseconds--}
```
public int getMilliseconds()
```


Restituisce la componente millisecondi dell'intervallo di tempo, rappresentata da questa istanza.

**Returns:**
int - la componente millisecondi dell'intervallo di tempo nell'intervallo da -999 a 999.
### getMinutes() {#getMinutes--}
```
public int getMinutes()
```


Restituisce la componente minuti dell'intervallo di tempo, rappresentata da questa istanza.

**Returns:**
int - la componente minuti dell'intervallo di tempo nell'intervallo da -59 a 59.
### getSeconds() {#getSeconds--}
```
public int getSeconds()
```


Restituisce la componente secondi dell'intervallo di tempo, rappresentata da questa istanza.

**Returns:**
int - la componente secondi dell'intervallo di tempo nell'intervallo da -59 a 59.
### getTotalDays() {#getTotalDays--}
```
public double getTotalDays()
```


Restituisce il valore dell'istanza corrente espresso in giorni interi e frazionari.

**Returns:**
double - il numero totale di giorni rappresentati da questa istanza.
### getTotalHours() {#getTotalHours--}
```
public double getTotalHours()
```


Restituisce il valore dell'istanza corrente espresso in ore intere e frazionarie.

**Returns:**
double - il numero totale di ore rappresentate da questa istanza.
### getTotalMilliseconds() {#getTotalMilliseconds--}
```
public double getTotalMilliseconds()
```


Restituisce il valore dell'istanza corrente espresso in millisecondi interi e frazionari.

**Returns:**
double - il numero totale di millisecondi rappresentati da questa istanza.
### getTotalMinutes() {#getTotalMinutes--}
```
public double getTotalMinutes()
```


Restituisce il valore dell'istanza corrente espresso in minuti interi e frazionari.

**Returns:**
double - il numero totale di minuti rappresentati da questa istanza.
### getTotalSeconds() {#getTotalSeconds--}
```
public double getTotalSeconds()
```


Restituisce il valore dell'istanza corrente espresso in secondi interi e frazionari.

**Returns:**
double - il numero totale di secondi rappresentati da questa istanza.
### hashCode() {#hashCode--}
```
public int hashCode()
```




**Returns:**
int - \{@inheritDoc\}
### negate() {#negate--}
```
public TimeDelta negate()
```


Restituisce un nuovo `TimeDelta` il cui valore è il valore negato di questa istanza.

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - A new object with the same numeric value as this instance, but with the opposite sign.
### parse(String s) {#parse-java.lang.String-}
```
public static TimeDelta parse(String s)
```


Converte la rappresentazione stringa di un intervallo di tempo nel suo equivalente `TimeDelta`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| s | java.lang.String | una stringa che specifica l'intervallo di tempo da convertire. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - a time interval that corresponds to `s`.
### subtract(TimeDelta other) {#subtract-com.aspose.tasks.TimeDelta-}
```
public TimeDelta subtract(TimeDelta other)
```


Restituisce un nuovo oggetto TimeDelta il cui valore è la differenza tra questa e le istanze `other`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | l'istanza da sottrarre. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - a new object that represents the value of this instance minus value of other instance.
### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String - \{@inheritDoc\}
### tryParse(String s, TimeDelta[] result) {#tryParse-java.lang.String-com.aspose.tasks.TimeDelta---}
```
public static boolean tryParse(String s, TimeDelta[] result)
```


Converte la rappresentazione stringa di un intervallo di tempo nel suo equivalente TimeDelta e restituisce un valore che indica se la conversione è riuscita.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| s | java.lang.String | una stringa che specifica l'intervallo di tempo da convertire. |
| result | [TimeDelta\[\]](../../com.aspose.tasks/timedelta) | questo array deve contenere almeno un elemento. Quando questo metodo restituisce, `result[0]` contiene un oggetto che rappresenta l'intervallo di tempo specificato da `s`, oppure un intervallo di tempo di lunghezza zero se la conversione è fallita. |

**Returns:**
boolean - `true` se s è stato convertito con successo; altrimenti, `false`.
