---
title: "CalendarException"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta periodi di tempo eccezionali in un calendario."
type: docs
weight: 43
url: /it/java/com.aspose.tasks/calendarexception/
---

**Inheritance:**
java.lang.Object
```
public final class CalendarException
```

Rappresenta periodi di tempo eccezionali in un calendario.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [CalendarException()](#CalendarException--) | Inizializza una nuova istanza della classe [CalendarException](../../com.aspose.tasks/calendarexception). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [checkException(Date dt)](#checkException-java.util.Date-) | Restituisce true se l'istanza specificata della struct java.util.Date è il giorno di eccezione. |
| [delete()](#delete--) | Elimina l'istanza Exception dall'oggetto CalendarExceptionCollection del calendario padre. |
| [getDayWorking()](#getDayWorking--) | Ottiene un valore che indica se la data specificata o il tipo di giorno è lavorativo. |
| [getDaysOfWeek()](#getDaysOfWeek--) | Ottiene la DayTypeCollection per questo oggetto. |
| [getEnteredByOccurrences()](#getEnteredByOccurrences--) | Ottiene un valore che indica se l'intervallo di ricorrenza è definito inserendo un numero di occorrenze. |
| [getExceptionDates()](#getExceptionDates--) | Restituisce le date in cui l'eccezione del calendario è applicabile. |
| [getFromDate()](#getFromDate--) | Ottiene l'inizio del periodo di eccezione. |
| [getMonth()](#getMonth--) | Ottiene il mese per cui è programmata una ricorrenza di eccezione. |
| [getMonthDay()](#getMonthDay--) | Ottiene il giorno del mese in cui è programmata una ricorrenza di eccezione. |
| [getMonthItem()](#getMonthItem--) | Ottiene l'elemento mese per cui è programmata una ricorrenza di eccezione. |
| [getMonthPosition()](#getMonthPosition--) | Ottiene la posizione di un elemento mese all'interno di un mese. |
| [getName()](#getName--) | Ottiene il nome dell'eccezione. |
| [getOccurrences()](#getOccurrences--) | Ottiene il numero di occorrenze per le quali l'eccezione del calendario è valida. |
| [getParentCalendar()](#getParentCalendar--) | Ottiene il calendario principale per questo oggetto. |
| [getPeriod()](#getPeriod--) | Ottiene il periodo di ricorrenza per l'eccezione. |
| [getToDate()](#getToDate--) | Ottiene la fine del periodo di eccezione. |
| [getType()](#getType--) | Ottiene il tipo di eccezione. |
| [getWorkingTime()](#getWorkingTime--) | Restituisce il tempo di lavoro per un'eccezione del calendario. |
| [getWorkingTimes()](#getWorkingTimes--) | Ottiene l'oggetto WorkingTimeCollection. |
| [setDayWorking(boolean value)](#setDayWorking-boolean-) | Imposta un valore che indica se la data specificata o il tipo di giorno è lavorativo. |
| [setEnteredByOccurrences(boolean value)](#setEnteredByOccurrences-boolean-) | Imposta un valore che indica se l'intervallo di ricorrenza è definito inserendo un numero di occorrenze. |
| [setFromDate(Date value)](#setFromDate-java.util.Date-) | Imposta l'inizio del tempo dell'eccezione. |
| [setMonth(int value)](#setMonth-int-) | Imposta il mese per cui è programmata una ricorrenza di eccezione. |
| [setMonthDay(int value)](#setMonthDay-int-) | Imposta il giorno del mese in cui è programmata una ricorrenza di eccezione. |
| [setMonthItem(int value)](#setMonthItem-int-) | Imposta l'elemento del mese per cui è programmata una ricorrenza di eccezione. |
| [setMonthPosition(int value)](#setMonthPosition-int-) | Imposta la posizione di un elemento del mese all'interno di un mese. |
| [setName(String value)](#setName-java.lang.String-) | Imposta il nome dell'eccezione. |
| [setOccurrences(int value)](#setOccurrences-int-) | Imposta il numero di occorrenze per le quali l'eccezione del calendario è valida. |
| [setPeriod(int value)](#setPeriod-int-) | Imposta il periodo di ricorrenza per l'eccezione. |
| [setToDate(Date value)](#setToDate-java.util.Date-) | Imposta la fine del tempo dell'eccezione. |
| [setType(int value)](#setType-int-) | Imposta il tipo di eccezione. |
| [setWorkingTimes(WorkingTimeCollection value)](#setWorkingTimes-com.aspose.tasks.WorkingTimeCollection-) | Imposta l'oggetto WorkingTimeCollection. |
### CalendarException() {#CalendarException--}
```
public CalendarException()
```


Inizializza una nuova istanza della classe [CalendarException](../../com.aspose.tasks/calendarexception).

### checkException(Date dt) {#checkException-java.util.Date-}
```
public final boolean checkException(Date dt)
```


Restituisce true se l'istanza specificata della struct java.util.Date è il giorno di eccezione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dt | java.util.Date | l'istanza specificata della struttura java.util.Date. |

**Returns:**
boolean - Restituisce true se il valore java.util.Date è il giorno dell'eccezione; altrimenti, false.
### delete() {#delete--}
```
public final void delete()
```


Elimina l'istanza Exception dall'oggetto CalendarExceptionCollection del calendario padre.

### getDayWorking() {#getDayWorking--}
```
public final boolean getDayWorking()
```


Ottiene un valore che indica se la data specificata o il tipo di giorno è lavorativo.

**Returns:**
boolean - un valore che indica se la data o il tipo di giorno specificato è lavorativo.
### getDaysOfWeek() {#getDaysOfWeek--}
```
public final DayTypeCollection getDaysOfWeek()
```


Ottiene la DayTypeCollection per questo oggetto. I giorni della settimana in cui l'eccezione è valida.

**Returns:**
[DayTypeCollection](../../com.aspose.tasks/daytypecollection) - the DayTypeCollection for this object.
### getEnteredByOccurrences() {#getEnteredByOccurrences--}
```
public final boolean getEnteredByOccurrences()
```


Ottiene un valore che indica se l'intervallo di ricorrenza è definito inserendo un numero di occorrenze. False specifica che l'intervallo di ricorrenza è definito inserendo una data di fine.

**Returns:**
boolean - un valore che indica se l'intervallo di ricorrenza è definito inserendo un numero di occorrenze.
### getExceptionDates() {#getExceptionDates--}
```
public final Iterable<Date> getExceptionDates()
```


Restituisce le date in cui l'eccezione del calendario è applicabile.

**Returns:**
java.lang.Iterable&lt;java.util.Date&gt; - date in cui l'eccezione del calendario è applicabile.
### getFromDate() {#getFromDate--}
```
public final Date getFromDate()
```


Ottiene l'inizio del periodo di eccezione.

**Returns:**
java.util.Date - l'inizio del tempo dell'eccezione.
### getMonth() {#getMonth--}
```
public final int getMonth()
```


Ottiene il mese per cui è programmata una ricorrenza di eccezione.

**Returns:**
int - il mese per cui è programmata una ricorrenza di eccezione.
### getMonthDay() {#getMonthDay--}
```
public final int getMonthDay()
```


Ottiene il giorno del mese in cui è programmata una ricorrenza di eccezione.

**Returns:**
int - il giorno del mese in cui è programmata una ricorrenza di eccezione.
### getMonthItem() {#getMonthItem--}
```
public final int getMonthItem()
```


Ottiene l'elemento mese per cui è programmata una ricorrenza di eccezione.

**Returns:**
int - l'elemento del mese per cui è programmata una ricorrenza di eccezione.
### getMonthPosition() {#getMonthPosition--}
```
public final int getMonthPosition()
```


Ottiene la posizione di un elemento mese all'interno di un mese.

**Returns:**
int - la posizione di un elemento del mese all'interno di un mese.
### getName() {#getName--}
```
public final String getName()
```


Ottiene il nome dell'eccezione.

**Returns:**
java.lang.String - il nome dell'eccezione.
### getOccurrences() {#getOccurrences--}
```
public final int getOccurrences()
```


Ottiene il numero di occorrenze per le quali l'eccezione del calendario è valida.

**Returns:**
int - il numero di occorrenze per le quali l'eccezione del calendario è valida.
### getParentCalendar() {#getParentCalendar--}
```
public final Calendar getParentCalendar()
```


Ottiene il calendario principale per questo oggetto.

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - the parent calendar for this object.
### getPeriod() {#getPeriod--}
```
public final int getPeriod()
```


Ottiene il periodo di ricorrenza per l'eccezione.

**Returns:**
int - il periodo di ricorrenza per l'eccezione.
### getToDate() {#getToDate--}
```
public final Date getToDate()
```


Ottiene la fine del periodo di eccezione.

**Returns:**
java.util.Date - la fine del tempo dell'eccezione.
### getType() {#getType--}
```
public final int getType()
```


Ottiene il tipo di eccezione.

**Returns:**
int - il tipo di eccezione.
### getWorkingTime() {#getWorkingTime--}
```
public final double getWorkingTime()
```


Restituisce il tempo di lavoro per un'eccezione del calendario.

**Returns:**
double - Restituisce il tempo di lavoro per questa eccezione del calendario.
### getWorkingTimes() {#getWorkingTimes--}
```
public final WorkingTimeCollection getWorkingTimes()
```


Ottiene l'oggetto WorkingTimeCollection. La collezione di tempi di lavoro che definisce il tempo lavorato nel giorno della settimana.

--------------------

Deve essere presente almeno un tempo di lavoro e non possono esserne più di cinque.

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - the WorkingTimeCollection object.
### setDayWorking(boolean value) {#setDayWorking-boolean-}
```
public final void setDayWorking(boolean value)
```


Imposta un valore che indica se la data specificata o il tipo di giorno è lavorativo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se la data o il tipo di giorno specificato è lavorativo. |

### setEnteredByOccurrences(boolean value) {#setEnteredByOccurrences-boolean-}
```
public final void setEnteredByOccurrences(boolean value)
```


Imposta un valore che indica se l'intervallo di ricorrenza è definito inserendo un numero di occorrenze. False specifica che l'intervallo di ricorrenza è definito inserendo una data di fine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se l'intervallo di ricorrenza è definito inserendo un numero di occorrenze. |

### setFromDate(Date value) {#setFromDate-java.util.Date-}
```
public final void setFromDate(Date value)
```


Imposta l'inizio del tempo dell'eccezione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date | l'inizio del tempo dell'eccezione. |

### setMonth(int value) {#setMonth-int-}
```
public final void setMonth(int value)
```


Imposta il mese per cui è programmata una ricorrenza di eccezione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | il mese per il quale è programmata una ricorrenza di eccezione. |

### setMonthDay(int value) {#setMonthDay-int-}
```
public final void setMonthDay(int value)
```


Imposta il giorno del mese in cui è programmata una ricorrenza di eccezione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | il giorno del mese in cui è programmata una ricorrenza di eccezione. |

### setMonthItem(int value) {#setMonthItem-int-}
```
public final void setMonthItem(int value)
```


Imposta l'elemento del mese per cui è programmata una ricorrenza di eccezione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | l'elemento del mese per il quale è programmata una ricorrenza di eccezione. |

### setMonthPosition(int value) {#setMonthPosition-int-}
```
public final void setMonthPosition(int value)
```


Imposta la posizione di un elemento del mese all'interno di un mese.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | la posizione di un elemento del mese all'interno di un mese. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Imposta il nome dell'eccezione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | il nome dell'eccezione. |

### setOccurrences(int value) {#setOccurrences-int-}
```
public final void setOccurrences(int value)
```


Imposta il numero di occorrenze per le quali l'eccezione del calendario è valida.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | il numero di occorrenze per le quali l'eccezione del calendario è valida. |

### setPeriod(int value) {#setPeriod-int-}
```
public final void setPeriod(int value)
```


Imposta il periodo di ricorrenza per l'eccezione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | il periodo di ricorrenza per l'eccezione. |

### setToDate(Date value) {#setToDate-java.util.Date-}
```
public final void setToDate(Date value)
```


Imposta la fine del tempo dell'eccezione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date | la fine del tempo dell'eccezione. |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


Imposta il tipo di eccezione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | il tipo di eccezione. |

### setWorkingTimes(WorkingTimeCollection value) {#setWorkingTimes-com.aspose.tasks.WorkingTimeCollection-}
```
public final void setWorkingTimes(WorkingTimeCollection value)
```


Imposta l'oggetto WorkingTimeCollection. La collezione di tempi di lavoro che definisce il tempo lavorato nel giorno della settimana.

--------------------

Deve essere presente almeno un tempo di lavoro e non possono esserne più di cinque.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) | l'oggetto WorkingTimeCollection. |

