---
title: "RecurringTaskInfo"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta i dettagli di un'attività ricorrente in un progetto."
type: docs
weight: 244
url: /it/java/com.aspose.tasks/recurringtaskinfo/
---

**Inheritance:**
java.lang.Object
```
public class RecurringTaskInfo
```

Rappresenta i dettagli di un'attività ricorrente in un progetto.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getDailyRepetitions()](#getDailyRepetitions--) | Restituisce un numero di ripetizioni per il modello di ricorrenza giornaliera. |
| [getDailyUseWorkdays()](#getDailyUseWorkdays--) | Restituisce un valore che indica se utilizzare i giorni lavorativi per il modello di ricorrenza giornaliera. |
| [getDuration()](#getDuration--) | Restituisce la durata per una singola occorrenza dell'attività ricorrente. |
| [getEndDate()](#getEndDate--) | Restituisce la data di fine delle occorrenze. |
| [getMonthlyDay()](#getMonthlyDay--) | Restituisce un numero di giorni del modello di ricorrenza mensile. |
| [getMonthlyOrdinalDay()](#getMonthlyOrdinalDay--) | Restituisce un giorno del modello di ricorrenza mensile quando si utilizza il giorno ordinal. |
| [getMonthlyOrdinalNumber()](#getMonthlyOrdinalNumber--) | Restituisce un numero ordinal del modello di ricorrenza mensile. |
| [getMonthlyOrdinalRepetitions()](#getMonthlyOrdinalRepetitions--) | Restituisce un numero di ripetizioni per il modello di ricorrenza mensile quando si utilizza il giorno ordinal. |
| [getMonthlyRepetitions()](#getMonthlyRepetitions--) | Restituisce un numero di ripetizioni per il modello di ricorrenza mensile. |
| [getMonthlyUseOrdinalDay()](#getMonthlyUseOrdinalDay--) | Restituisce un valore che indica se utilizzare il giorno ordinal per il modello di ricorrenza mensile. |
| [getOccurrences()](#getOccurrences--) | Restituisce un numero di occorrenze dell'attività ricorrente. |
| [getRecurrencePattern()](#getRecurrencePattern--) | Restituisce un modello di ricorrenza dell'attività ricorrente. |
| [getStartDate()](#getStartDate--) | Restituisce la data di inizio delle occorrenze. |
| [getTask()](#getTask--) | Restituisce l'attività padre di questa istanza della classe [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo). |
| [getUseEndDate()](#getUseEndDate--) | Restituisce un valore che indica se utilizzare la data di fine o un numero di occorrenze per l'attività ricorrente. |
| [getWeeklyDays()](#getWeeklyDays--) | Restituisce una raccolta di giorni utilizzati nel modello di ricorrenza settimanale. |
| [getWeeklyRepetitions()](#getWeeklyRepetitions--) | Restituisce un numero di ripetizioni per il modello di ricorrenza settimanale. |
| [getYearlyDate()](#getYearlyDate--) | Restituisce una data per il modello di ricorrenza annuale. |
| [getYearlyOrdinalDay()](#getYearlyOrdinalDay--) | Ottiene un giorno della settimana del modello di ricorrenza annuale quando si utilizza il giorno ordinal. |
| [getYearlyOrdinalMonth()](#getYearlyOrdinalMonth--) | Ottiene un mese del modello di ricorrenza annuale quando si utilizza il giorno ordinal. |
| [getYearlyOrdinalNumber()](#getYearlyOrdinalNumber--) | Ottiene un numero ordinal del modello di ricorrenza annuale. |
| [getYearlyUseOrdinalDay()](#getYearlyUseOrdinalDay--) | Ottiene un valore che indica se utilizzare il giorno ordinal per il modello di ricorrenza annuale. |
| [setDailyRepetitions(int value)](#setDailyRepetitions-int-) | Imposta un numero di ripetizioni per il modello di ricorrenza giornaliera. |
| [setDailyUseWorkdays(boolean value)](#setDailyUseWorkdays-boolean-) | Imposta un valore che indica se utilizzare i giorni lavorativi per il modello di ricorrenza giornaliera. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Imposta la durata per una singola occorrenza dell'attività ricorrente. |
| [setEndDate(Date value)](#setEndDate-java.util.Date-) | Imposta la data di fine delle occorrenze. |
| [setMonthlyDay(int value)](#setMonthlyDay-int-) | Imposta un numero di giorni del modello di ricorrenza mensile. |
| [setMonthlyOrdinalDay(int value)](#setMonthlyOrdinalDay-int-) | Imposta un giorno del modello di ricorrenza mensile quando si utilizza il giorno ordinal. |
| [setMonthlyOrdinalNumber(int value)](#setMonthlyOrdinalNumber-int-) | Imposta un numero ordinal del modello di ricorrenza mensile. |
| [setMonthlyOrdinalRepetitions(int value)](#setMonthlyOrdinalRepetitions-int-) | Imposta un numero di ripetizioni per il modello di ricorrenza mensile quando si utilizza il giorno ordinal. |
| [setMonthlyRepetitions(int value)](#setMonthlyRepetitions-int-) | Imposta un numero di ripetizioni per il modello di ricorrenza mensile. |
| [setMonthlyUseOrdinalDay(boolean value)](#setMonthlyUseOrdinalDay-boolean-) | Imposta un valore che indica se utilizzare il giorno ordinal per il modello di ricorrenza mensile. |
| [setOccurrences(int value)](#setOccurrences-int-) | Imposta un numero di occorrenze dell'attività ricorrente. |
| [setRecurrencePattern(int value)](#setRecurrencePattern-int-) | Imposta un modello di ricorrenza dell'attività ricorrente. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Imposta la data di inizio delle occorrenze. |
| [setUseEndDate(boolean value)](#setUseEndDate-boolean-) | Imposta un valore che indica se utilizzare la data di fine o un numero di occorrenze per l'attività ricorrente. |
| [setWeeklyDays(int value)](#setWeeklyDays-int-) | Imposta una raccolta di giorni utilizzati nel modello di ricorrenza settimanale. |
| [setWeeklyRepetitions(int value)](#setWeeklyRepetitions-int-) | Imposta un numero di ripetizioni per il modello di ricorrenza settimanale. |
| [setYearlyDate(Date value)](#setYearlyDate-java.util.Date-) | Imposta una data per il modello di ricorrenza annuale. |
| [setYearlyOrdinalDay(int value)](#setYearlyOrdinalDay-int-) | Imposta un giorno della settimana del modello di ricorrenza annuale quando si utilizza il giorno ordinal. |
| [setYearlyOrdinalMonth(int value)](#setYearlyOrdinalMonth-int-) | Imposta un mese del modello di ricorrenza annuale quando si utilizza il giorno ordinal. |
| [setYearlyOrdinalNumber(int value)](#setYearlyOrdinalNumber-int-) | Imposta un numero ordinal del modello di ricorrenza annuale. |
| [setYearlyUseOrdinalDay(boolean value)](#setYearlyUseOrdinalDay-boolean-) | Imposta un valore che indica se utilizzare il giorno ordinal per il modello di ricorrenza annuale. |
### getDailyRepetitions() {#getDailyRepetitions--}
```
public final int getDailyRepetitions()
```


Restituisce un numero di ripetizioni per il modello di ricorrenza giornaliera.

**Returns:**
int - un numero di ripetizioni per il modello di ricorrenza giornaliera.
### getDailyUseWorkdays() {#getDailyUseWorkdays--}
```
public final boolean getDailyUseWorkdays()
```


Restituisce un valore che indica se utilizzare i giorni lavorativi per il modello di ricorrenza giornaliera.

**Returns:**
boolean - un valore che indica se utilizzare i giorni lavorativi per il modello di ricorrenza giornaliera.
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Restituisce la durata per una singola occorrenza dell'attività ricorrente.

--------------------

l'istanza della classe `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskinfo\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskinfo\#setDuration-Duration-)).

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the duration for one occurrence of the recurring task.
### getEndDate() {#getEndDate--}
```
public final Date getEndDate()
```


Restituisce la data di fine delle occorrenze.

**Returns:**
java.util.Date - la data di fine delle occorrenze.
### getMonthlyDay() {#getMonthlyDay--}
```
public final int getMonthlyDay()
```


Restituisce un numero di giorni del modello di ricorrenza mensile.

**Returns:**
int - un numero di giorno del modello di ricorrenza mensile.
### getMonthlyOrdinalDay() {#getMonthlyOrdinalDay--}
```
public final int getMonthlyOrdinalDay()
```


Restituisce un giorno del modello di ricorrenza mensile quando si utilizza il giorno ordinal.

--------------------

Può essere uno dei valori dell'enumerazione [DayOfWeek](../../com.aspose.tasks/dayofweek).

**Returns:**
int - un giorno del modello di ricorrenza mensile quando si utilizza il giorno ordinal.
### getMonthlyOrdinalNumber() {#getMonthlyOrdinalNumber--}
```
public final int getMonthlyOrdinalNumber()
```


Restituisce un numero ordinal del modello di ricorrenza mensile.

--------------------

Può essere uno dei valori dell'enumerazione [OrdinalNumber](../../com.aspose.tasks/ordinalnumber).

**Returns:**
int - un numero ordinal del modello di ricorrenza mensile.
### getMonthlyOrdinalRepetitions() {#getMonthlyOrdinalRepetitions--}
```
public final int getMonthlyOrdinalRepetitions()
```


Restituisce un numero di ripetizioni per il modello di ricorrenza mensile quando si utilizza il giorno ordinal.

**Returns:**
int - un numero di ripetizioni per il modello di ricorrenza mensile quando si utilizza il giorno ordinal.
### getMonthlyRepetitions() {#getMonthlyRepetitions--}
```
public final int getMonthlyRepetitions()
```


Restituisce un numero di ripetizioni per il modello di ricorrenza mensile.

**Returns:**
int - un numero di ripetizioni per il modello di ricorrenza mensile.
### getMonthlyUseOrdinalDay() {#getMonthlyUseOrdinalDay--}
```
public final boolean getMonthlyUseOrdinalDay()
```


Restituisce un valore che indica se utilizzare il giorno ordinal per il modello di ricorrenza mensile.

**Returns:**
boolean - un valore che indica se utilizzare il giorno ordinal per il modello di ricorrenza mensile.
### getOccurrences() {#getOccurrences--}
```
public final int getOccurrences()
```


Restituisce un numero di occorrenze dell'attività ricorrente.

**Returns:**
int - un numero di occorrenze del compito ricorrente.
### getRecurrencePattern() {#getRecurrencePattern--}
```
public final int getRecurrencePattern()
```


Restituisce un modello di ricorrenza dell'attività ricorrente.

--------------------

Può essere uno dei valori dell'enumerazione `RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskinfo\#getRecurrencePattern--)/[setRecurrencePattern(int)](../../com.aspose.tasks/recurringtaskinfo\#setRecurrencePattern-int-)).

**Returns:**
int - un modello di ricorrenza del compito ricorrente.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


Restituisce la data di inizio delle occorrenze.

**Returns:**
java.util.Date - la data di inizio delle occorrenze.
### getTask() {#getTask--}
```
public final Task getTask()
```


Restituisce l'attività padre di questa istanza della classe [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo).

**Returns:**
[Task](../../com.aspose.tasks/task) - the parent task of this instance of [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) class.
### getUseEndDate() {#getUseEndDate--}
```
public final boolean getUseEndDate()
```


Restituisce un valore che indica se utilizzare la data di fine o un numero di occorrenze per l'attività ricorrente.

**Returns:**
boolean - un valore che indica se utilizzare la data di fine o un numero di occorrenze per il compito ricorrente.
### getWeeklyDays() {#getWeeklyDays--}
```
public final int getWeeklyDays()
```


Restituisce una raccolta di giorni utilizzati nel modello di ricorrenza settimanale.

--------------------

**Returns:**
int - una raccolta di giorni utilizzati nel modello di ricorrenza settimanale.
### getWeeklyRepetitions() {#getWeeklyRepetitions--}
```
public final int getWeeklyRepetitions()
```


Restituisce un numero di ripetizioni per il modello di ricorrenza settimanale.

**Returns:**
int - un numero di ripetizioni per il modello di ricorrenza settimanale.
### getYearlyDate() {#getYearlyDate--}
```
public final Date getYearlyDate()
```


Restituisce una data per il modello di ricorrenza annuale.

**Returns:**
java.util.Date - una data per il modello di ricorrenza annuale.
### getYearlyOrdinalDay() {#getYearlyOrdinalDay--}
```
public final int getYearlyOrdinalDay()
```


Ottiene un giorno della settimana del modello di ricorrenza annuale quando si utilizza il giorno ordinal.

--------------------

Può essere uno dei valori dell'enumerazione [DayOfWeek](../../com.aspose.tasks/dayofweek).

**Returns:**
int - un giorno della settimana del modello di ricorrenza annuale quando si utilizza il giorno ordinal.
### getYearlyOrdinalMonth() {#getYearlyOrdinalMonth--}
```
public final int getYearlyOrdinalMonth()
```


Ottiene un mese del modello di ricorrenza annuale quando si utilizza il giorno ordinal.

--------------------

Può essere uno dei valori dell'enumerazione [Month](../../com.aspose.tasks/month).

**Returns:**
int - un mese del modello di ricorrenza annuale quando si utilizza il giorno ordinal.
### getYearlyOrdinalNumber() {#getYearlyOrdinalNumber--}
```
public final int getYearlyOrdinalNumber()
```


Ottiene un numero ordinal del modello di ricorrenza annuale.

--------------------

Può essere uno dei valori dell'enumerazione [OrdinalNumber](../../com.aspose.tasks/ordinalnumber).

**Returns:**
int - un numero ordinal del modello di ricorrenza annuale.
### getYearlyUseOrdinalDay() {#getYearlyUseOrdinalDay--}
```
public final boolean getYearlyUseOrdinalDay()
```


Ottiene un valore che indica se utilizzare il giorno ordinal per il modello di ricorrenza annuale.

**Returns:**
boolean - un valore che indica se utilizzare il giorno ordinal per il modello di ricorrenza annuale.
### setDailyRepetitions(int value) {#setDailyRepetitions-int-}
```
public final void setDailyRepetitions(int value)
```


Imposta un numero di ripetizioni per il modello di ricorrenza giornaliera.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | un numero di ripetizioni per il modello di ricorrenza giornaliera. |

### setDailyUseWorkdays(boolean value) {#setDailyUseWorkdays-boolean-}
```
public final void setDailyUseWorkdays(boolean value)
```


Imposta un valore che indica se utilizzare i giorni lavorativi per il modello di ricorrenza giornaliera.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se utilizzare i giorni lavorativi per il modello di ricorrenza giornaliera. |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Imposta la durata per una singola occorrenza dell'attività ricorrente.

--------------------

l'istanza della classe `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskinfo\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskinfo\#setDuration-Duration-)).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | la durata per una singola occorrenza dell'attività ricorrente. |

### setEndDate(Date value) {#setEndDate-java.util.Date-}
```
public final void setEndDate(Date value)
```


Imposta la data di fine delle occorrenze.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date | la data di fine delle occorrenze. |

### setMonthlyDay(int value) {#setMonthlyDay-int-}
```
public final void setMonthlyDay(int value)
```


Imposta un numero di giorni del modello di ricorrenza mensile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | un numero di giorni del modello di ricorrenza mensile. |

### setMonthlyOrdinalDay(int value) {#setMonthlyOrdinalDay-int-}
```
public final void setMonthlyOrdinalDay(int value)
```


Imposta un giorno del modello di ricorrenza mensile quando si utilizza il giorno ordinal.

--------------------

Può essere uno dei valori dell'enumerazione [DayOfWeek](../../com.aspose.tasks/dayofweek).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | un giorno del modello di ricorrenza mensile quando si utilizza il giorno ordinal. |

### setMonthlyOrdinalNumber(int value) {#setMonthlyOrdinalNumber-int-}
```
public final void setMonthlyOrdinalNumber(int value)
```


Imposta un numero ordinal del modello di ricorrenza mensile.

--------------------

Può essere uno dei valori dell'enumerazione [OrdinalNumber](../../com.aspose.tasks/ordinalnumber).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | un numero ordinal del modello di ricorrenza mensile. |

### setMonthlyOrdinalRepetitions(int value) {#setMonthlyOrdinalRepetitions-int-}
```
public final void setMonthlyOrdinalRepetitions(int value)
```


Imposta un numero di ripetizioni per il modello di ricorrenza mensile quando si utilizza il giorno ordinal.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | un numero di ripetizioni per il modello di ricorrenza mensile quando si utilizza il giorno ordinal. |

### setMonthlyRepetitions(int value) {#setMonthlyRepetitions-int-}
```
public final void setMonthlyRepetitions(int value)
```


Imposta un numero di ripetizioni per il modello di ricorrenza mensile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | un numero di ripetizioni per il modello di ricorrenza mensile. |

### setMonthlyUseOrdinalDay(boolean value) {#setMonthlyUseOrdinalDay-boolean-}
```
public final void setMonthlyUseOrdinalDay(boolean value)
```


Imposta un valore che indica se utilizzare il giorno ordinal per il modello di ricorrenza mensile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se utilizzare il giorno ordinal per il modello di ricorrenza mensile. |

### setOccurrences(int value) {#setOccurrences-int-}
```
public final void setOccurrences(int value)
```


Imposta un numero di occorrenze dell'attività ricorrente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | un numero di occorrenze dell'attività ricorrente. |

### setRecurrencePattern(int value) {#setRecurrencePattern-int-}
```
public final void setRecurrencePattern(int value)
```


Imposta un modello di ricorrenza dell'attività ricorrente.

--------------------

Può essere uno dei valori dell'enumerazione `RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskinfo\#getRecurrencePattern--)/[setRecurrencePattern(int)](../../com.aspose.tasks/recurringtaskinfo\#setRecurrencePattern-int-)).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | un modello di ricorrenza dell'attività ricorrente. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


Imposta la data di inizio delle occorrenze.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date | la data di inizio delle occorrenze. |

### setUseEndDate(boolean value) {#setUseEndDate-boolean-}
```
public final void setUseEndDate(boolean value)
```


Imposta un valore che indica se utilizzare la data di fine o un numero di occorrenze per l'attività ricorrente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se utilizzare la data di fine o un numero di occorrenze per l'attività ricorrente. |

### setWeeklyDays(int value) {#setWeeklyDays-int-}
```
public final void setWeeklyDays(int value)
```


Imposta una raccolta di giorni utilizzati nel modello di ricorrenza settimanale.

--------------------

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | una raccolta di giorni utilizzati nel modello di ricorrenza settimanale. |

### setWeeklyRepetitions(int value) {#setWeeklyRepetitions-int-}
```
public final void setWeeklyRepetitions(int value)
```


Imposta un numero di ripetizioni per il modello di ricorrenza settimanale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | un numero di ripetizioni per il modello di ricorrenza settimanale. |

### setYearlyDate(Date value) {#setYearlyDate-java.util.Date-}
```
public final void setYearlyDate(Date value)
```


Imposta una data per il modello di ricorrenza annuale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date | una data per il modello di ricorrenza annuale. |

### setYearlyOrdinalDay(int value) {#setYearlyOrdinalDay-int-}
```
public final void setYearlyOrdinalDay(int value)
```


Imposta un giorno della settimana del modello di ricorrenza annuale quando si utilizza il giorno ordinal.

--------------------

Può essere uno dei valori dell'enumerazione [DayOfWeek](../../com.aspose.tasks/dayofweek).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | un giorno della settimana del modello di ricorrenza annuale quando si utilizza il giorno ordinal. |

### setYearlyOrdinalMonth(int value) {#setYearlyOrdinalMonth-int-}
```
public final void setYearlyOrdinalMonth(int value)
```


Imposta un mese del modello di ricorrenza annuale quando si utilizza il giorno ordinal.

--------------------

Può essere uno dei valori dell'enumerazione [Month](../../com.aspose.tasks/month).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | un mese del modello di ricorrenza annuale quando si utilizza il giorno ordinal. |

### setYearlyOrdinalNumber(int value) {#setYearlyOrdinalNumber-int-}
```
public final void setYearlyOrdinalNumber(int value)
```


Imposta un numero ordinal del modello di ricorrenza annuale.

--------------------

Può essere uno dei valori dell'enumerazione [OrdinalNumber](../../com.aspose.tasks/ordinalnumber).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | un numero ordinal del modello di ricorrenza annuale. |

### setYearlyUseOrdinalDay(boolean value) {#setYearlyUseOrdinalDay-boolean-}
```
public final void setYearlyUseOrdinalDay(boolean value)
```


Imposta un valore che indica se utilizzare il giorno ordinal per il modello di ricorrenza annuale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se utilizzare il giorno ordinal per il modello di ricorrenza annuale. |

