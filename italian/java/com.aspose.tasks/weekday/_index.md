---
title: "WeekDay"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta un giorno della settimana che definisce sia i giorni regolari di una settimana sia i giorni di eccezione in un calendario."
type: docs
weight: 352
url: /it/java/com.aspose.tasks/weekday/
---

**Inheritance:**
java.lang.Object
```
public class WeekDay
```

Rappresenta un giorno della settimana che definisce sia i giorni regolari di una settimana sia i giorni di eccezione in un calendario.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [WeekDay(int dayType)](#WeekDay-int-) | Inizializza una nuova istanza della classe [WeekDay](../../com.aspose.tasks/weekday) con il tipo di giorno specificato. |
| [WeekDay(int dayType, List&lt;WorkingTime&gt; workingTimes)](#WeekDay-int-java.util.List-com.aspose.tasks.WorkingTime--) | Inizializza una nuova istanza della classe [WeekDay](../../com.aspose.tasks/weekday) con il tipo di giorno specificato e l'elenco dei periodi di lavoro. |
| [WeekDay(int dayType, WorkingTime[] workingTimes)](#WeekDay-int-com.aspose.tasks.WorkingTime...-) | Inizializza una nuova istanza della classe [WeekDay](../../com.aspose.tasks/weekday) con il tipo di giorno specificato e i periodi di lavoro. |
| [WeekDay()](#WeekDay--) | Inizializza una nuova istanza della classe [WeekDay](../../com.aspose.tasks/weekday). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [castToDayType(int dw)](#castToDayType-int-) | Converte il [DayOfWeek](../../com.aspose.tasks/dayofweek) di .Net in `DayType`([getDayType()](../../com.aspose.tasks/weekday\#getDayType--)/[setDayType(int)](../../com.aspose.tasks/weekday\#setDayType-int-)). |
| [createDefaultWorkingDay(int dayType)](#createDefaultWorkingDay-int-) | Crea un giorno lavorativo predefinito. |
| [deepClone()](#deepClone--) | Restituisce una copia profonda del giorno della settimana. |
| [equals(Object obj)](#equals-java.lang.Object-) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| [getDayType()](#getDayType--) | Ottiene il tipo di un giorno. |
| [getDayWorking()](#getDayWorking--) | Ottiene un valore che indica se la data specificata o il tipo di giorno è lavorativo. |
| [getFromDate()](#getFromDate--) | Ottiene l'inizio di un periodo di eccezione. |
| [getToDate()](#getToDate--) | Ottiene la fine di un periodo di eccezione. |
| [getWorkingTime()](#getWorkingTime--) | Restituisce il tempo lavorativo per un giorno della settimana. |
| [getWorkingTimes()](#getWorkingTimes--) | Ottiene la WorkingTimeCollection per questa istanza di WeekDay. |
| [hashCode()](#hashCode--) | Restituisce un valore di codice hash per l'istanza della classe [WeekDay](../../com.aspose.tasks/weekday). |
| [setDayWorking(boolean value)](#setDayWorking-boolean-) | Imposta un valore che indica se la data specificata o il tipo di giorno è lavorativo. |
| [setDefaultWorkingTime(WeekDay day)](#setDefaultWorkingTime-com.aspose.tasks.WeekDay-) | Imposta i periodi di tempo predefiniti per il giorno della settimana specificato. |
| [setFromDate(Date value)](#setFromDate-java.util.Date-) | Imposta l'inizio di un periodo di eccezione. |
| [setToDate(Date value)](#setToDate-java.util.Date-) | Imposta la fine di un periodo di eccezione. |
### WeekDay(int dayType) {#WeekDay-int-}
```
public WeekDay(int dayType)
```


Inizializza una nuova istanza della classe [WeekDay](../../com.aspose.tasks/weekday) con il tipo di giorno specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dayType | int | Il tipo di giorno specificato. |

### WeekDay(int dayType, List&lt;WorkingTime&gt; workingTimes) {#WeekDay-int-java.util.List-com.aspose.tasks.WorkingTime--}
```
public WeekDay(int dayType, List<WorkingTime> workingTimes)
```


Inizializza una nuova istanza della classe [WeekDay](../../com.aspose.tasks/weekday) con il tipo di giorno specificato e l'elenco dei periodi di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dayType | int | Il tipo di giorno specificato. |
| workingTimes | java.util.List&lt;com.aspose.tasks.WorkingTime&gt; | Elenco dei periodi di tempo lavorativi. |

### WeekDay(int dayType, WorkingTime[] workingTimes) {#WeekDay-int-com.aspose.tasks.WorkingTime...-}
```
public WeekDay(int dayType, WorkingTime[] workingTimes)
```


Inizializza una nuova istanza della classe [WeekDay](../../com.aspose.tasks/weekday) con il tipo di giorno specificato e i periodi di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dayType | int | Il tipo di giorno specificato. |
| workingTimes | [WorkingTime\[\]](../../com.aspose.tasks/workingtime) | Array dei periodi di tempo lavorativi. |

### WeekDay() {#WeekDay--}
```
public WeekDay()
```


Inizializza una nuova istanza della classe [WeekDay](../../com.aspose.tasks/weekday).

### castToDayType(int dw) {#castToDayType-int-}
```
public static int castToDayType(int dw)
```


Converte il [DayOfWeek](../../com.aspose.tasks/dayofweek) di .Net in `DayType`([getDayType()](../../com.aspose.tasks/weekday\#getDayType--)/[setDayType(int)](../../com.aspose.tasks/weekday\#setDayType-int-)).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dw | int | Il giorno della settimana da cui convertire. |

**Returns:**
int - Un tipo di giorno convertito.
### createDefaultWorkingDay(int dayType) {#createDefaultWorkingDay-int-}
```
public static WeekDay createDefaultWorkingDay(int dayType)
```


Crea un giorno lavorativo predefinito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dayType | int | Il tipo di giorno da cui creare il giorno lavorativo predefinito. |

**Returns:**
[WeekDay](../../com.aspose.tasks/weekday) - A default working day with working times 8-12 and 13-17.
### deepClone() {#deepClone--}
```
public final WeekDay deepClone()
```


Restituisce una copia profonda del giorno della settimana.

**Returns:**
[WeekDay](../../com.aspose.tasks/weekday) - Returns the deep copy of the week day.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | java.lang.Object | L'oggetto da confrontare con questa istanza. |

**Returns:**
boolean - **True** se l'oggetto specificato è un WeekDay che ha gli stessi valori FromDate, ToDate e WorkingTimes di questa istanza; altrimenti, **false**.
### getDayType() {#getDayType--}
```
public final int getDayType()
```


Ottiene il tipo di un giorno.

**Returns:**
int - il tipo di giorno.
### getDayWorking() {#getDayWorking--}
```
public final boolean getDayWorking()
```


Ottiene un valore che indica se la data specificata o il tipo di giorno è lavorativo.

**Returns:**
boolean - un valore che indica se la data o il tipo di giorno specificato è lavorativo.
### getFromDate() {#getFromDate--}
```
public final Date getFromDate()
```


Ottiene l'inizio di un periodo di eccezione.

**Returns:**
java.util.Date - l'inizio di un periodo di eccezione.
### getToDate() {#getToDate--}
```
public final Date getToDate()
```


Ottiene la fine di un periodo di eccezione.

**Returns:**
java.util.Date - la fine di un periodo di eccezione.
### getWorkingTime() {#getWorkingTime--}
```
public final double getWorkingTime()
```


Restituisce il tempo lavorativo per un giorno della settimana.

**Returns:**
double - Tempo di lavoro.
### getWorkingTimes() {#getWorkingTimes--}
```
public final WorkingTimeCollection getWorkingTimes()
```


Ottiene WorkingTimeCollection per questa istanza di WeekDay. La raccolta di tempi di lavoro che definiscono il tempo lavorato nel giorno della settimana.

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - WorkingTimeCollection for this WeekDay instance.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Restituisce un valore di codice hash per l'istanza della classe [WeekDay](../../com.aspose.tasks/weekday).

**Returns:**
int - restituisce un valore di codice hash per questo oggetto.
### setDayWorking(boolean value) {#setDayWorking-boolean-}
```
public final void setDayWorking(boolean value)
```


Imposta un valore che indica se la data specificata o il tipo di giorno è lavorativo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se la data o il tipo di giorno specificato è lavorativo. |

### setDefaultWorkingTime(WeekDay day) {#setDefaultWorkingTime-com.aspose.tasks.WeekDay-}
```
public static void setDefaultWorkingTime(WeekDay day)
```


Imposta i periodi di tempo predefiniti per il giorno della settimana specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| day | [WeekDay](../../com.aspose.tasks/weekday) | Il giorno della settimana su cui impostare il giorno lavorativo predefinito. |

### setFromDate(Date value) {#setFromDate-java.util.Date-}
```
public final void setFromDate(Date value)
```


Imposta l'inizio di un periodo di eccezione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date | l'inizio di un periodo di eccezione. |

### setToDate(Date value) {#setToDate-java.util.Date-}
```
public final void setToDate(Date value)
```


Imposta la fine di un periodo di eccezione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date | la fine di un periodo di eccezione. |

