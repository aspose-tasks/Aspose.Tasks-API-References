---
title: "TaskBaseline"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar Baseline för en uppgift."
type: docs
weight: 291
url: /sv/java/com.aspose.tasks/taskbaseline/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.Baseline](../../com.aspose.tasks/baseline)

**All Implemented Interfaces:**
java.lang.Comparable
```
public class TaskBaseline extends Baseline implements Comparable<Baseline>
```

Representerar Baseline för en uppgift.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [TaskBaseline(Task task)](#TaskBaseline-com.aspose.tasks.Task-) | Initierar en ny instans av klassen [TaskBaseline](../../com.aspose.tasks/taskbaseline). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [compareTo(TaskBaseline other)](#compareTo-com.aspose.tasks.TaskBaseline-) | Implementering av IComparable‑gränssnittet. |
| [equals(TaskBaseline other)](#equals-com.aspose.tasks.TaskBaseline-) | Returnerar ett värde som indikerar om denna instans är lika med det angivna TaskBaseline-objektet. |
| [equals(Object obj)](#equals-java.lang.Object-) | Returnerar ett värde som anger om detta objekt är lika med ett angivet objekt. |
| [getDuration()](#getDuration--) | Hämtar den schemalagda varaktigheten för uppgiften när baslinjen sparades. |
| [getEstimatedDuration()](#getEstimatedDuration--) | Hämtar ett värde som indikerar om baslinjevaraktigheten för uppgiften var uppskattad. |
| [getFinish()](#getFinish--) | Hämtar det schemalagda slutdatumet för uppgiften när baslinjen sparades. |
| [getFixedCost()](#getFixedCost--) | Hämtar en fast kostnad för uppgiften när baslinjen sparades. |
| [getInterim()](#getInterim--) | Hämtar ett värde som indikerar om detta är en interimbaslinje. |
| [getStart()](#getStart--) | Hämtar det planerade startdatumet för uppgiften när baslinjen sparades. |
| [getTimephasedData()](#getTimephasedData--) | Hämtar en TimephasedDataCollection-instans för detta objekt. |
| [hashCode()](#hashCode--) | Returnerar ett hashkodvärde för instansen av klassen [TaskBaseline](../../com.aspose.tasks/taskbaseline). |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Ställer in den planerade varaktigheten för uppgiften när baslinjen sparades. |
| [setEstimatedDuration(boolean value)](#setEstimatedDuration-boolean-) | Ställer in ett värde som indikerar om baslinjens varaktighet för uppgiften var uppskattad. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Ställer in det planerade slutdatumet för uppgiften när baslinjen sparades. |
| [setFixedCost(double value)](#setFixedCost-double-) | Ställer in en fast kostnad för uppgiften när baslinjen sparades. |
| [setInterim(boolean value)](#setInterim-boolean-) | Ställer in ett värde som indikerar om detta är en interimbaslinje. |
| [setStart(Date value)](#setStart-java.util.Date-) | Ställer in det planerade startdatumet för uppgiften när baslinjen sparades. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | Ställer in en TimephasedDataCollection-instans för detta objekt. |
### TaskBaseline(Task task) {#TaskBaseline-com.aspose.tasks.Task-}
```
public TaskBaseline(Task task)
```


Initierar en ny instans av klassen [TaskBaseline](../../com.aspose.tasks/taskbaseline).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Baslinjens överordnade uppgift. |

### compareTo(TaskBaseline other) {#compareTo-com.aspose.tasks.TaskBaseline-}
```
public final int compareTo(TaskBaseline other)
```


Implementering av IComparable‑gränssnittet. Jämför denna instans med det angivna Baseline‑objektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| other | [TaskBaseline](../../com.aspose.tasks/taskbaseline) | det angivna Baseline‑objektet att jämföra denna instans med. |

**Returns:**
int – returnerar -1 om denna instans är mindre än det angivna objektet, 1 om den är större än det angivna objektet; annars returneras 0.
### equals(TaskBaseline other) {#equals-com.aspose.tasks.TaskBaseline-}
```
public final boolean equals(TaskBaseline other)
```


Returnerar ett värde som indikerar om denna instans är lika med det angivna TaskBaseline-objektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| other | [TaskBaseline](../../com.aspose.tasks/taskbaseline) | det angivna AssignmentBaseline-objektet att jämföra med denna instans. |

**Returns:**
boolean - returnerar true om denna instans är lika med det angivna TaskBaseline-objektet; annars false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Returnerar ett värde som anger om detta objekt är lika med ett angivet objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | java.lang.Object | Objektet att jämföra med denna instans. |

**Returns:**
boolean - **True** om det angivna objektet är en TaskBaseline som har samma UID‑värde som denna instans; annars **false**.
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Hämtar den schemalagda varaktigheten för uppgiften när baslinjen sparades.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the scheduled duration of the task when the baseline was saved.
### getEstimatedDuration() {#getEstimatedDuration--}
```
public final boolean getEstimatedDuration()
```


Hämtar ett värde som indikerar om baslinjevaraktigheten för uppgiften var uppskattad.

**Returns:**
boolean - ett värde som indikerar om baslinjens varaktighet för uppgiften var uppskattad.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Hämtar det schemalagda slutdatumet för uppgiften när baslinjen sparades.

**Returns:**
java.util.Date - det planerade slutdatumet för uppgiften när baslinjen sparades.
### getFixedCost() {#getFixedCost--}
```
public final double getFixedCost()
```


Hämtar en fast kostnad för uppgiften när baslinjen sparades.

**Returns:**
double - en fast kostnad för uppgiften när baslinjen sparades.
### getInterim() {#getInterim--}
```
public final boolean getInterim()
```


Hämtar ett värde som indikerar om detta är en interimbaslinje.

**Returns:**
boolean - ett värde som indikerar om detta är en interimbaslinje.
### getStart() {#getStart--}
```
public final Date getStart()
```


Hämtar det planerade startdatumet för uppgiften när baslinjen sparades.

**Returns:**
java.util.Date - det planerade startdatumet för uppgiften när baslinjen sparades.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


Hämtar en TimephasedDataCollection-instans för detta objekt. Den tidsfasade data som är associerad med uppgiftsbaslinjen.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - a TimephasedDataCollection instance for this object.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Returnerar ett hashkodvärde för instansen av klassen [TaskBaseline](../../com.aspose.tasks/taskbaseline).

**Returns:**
int - returnerar ett hash‑kodvärde för detta objekt.
### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Ställer in den planerade varaktigheten för uppgiften när baslinjen sparades.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | den planerade varaktigheten för uppgiften när baslinjen sparades. |

### setEstimatedDuration(boolean value) {#setEstimatedDuration-boolean-}
```
public final void setEstimatedDuration(boolean value)
```


Ställer in ett värde som indikerar om baslinjens varaktighet för uppgiften var uppskattad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om baslinjens varaktighet för uppgiften var uppskattad. |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Ställer in det planerade slutdatumet för uppgiften när baslinjen sparades.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date | det planerade slutdatumet för uppgiften när baslinjen sparades. |

### setFixedCost(double value) {#setFixedCost-double-}
```
public final void setFixedCost(double value)
```


Ställer in en fast kostnad för uppgiften när baslinjen sparades.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double | en fast kostnad för uppgiften när baslinjen sparades. |

### setInterim(boolean value) {#setInterim-boolean-}
```
public final void setInterim(boolean value)
```


Ställer in ett värde som indikerar om detta är en interimbaslinje.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om detta är en interimistisk baslinje. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Ställer in det planerade startdatumet för uppgiften när baslinjen sparades.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date | det planerade startdatumet för uppgiften när baslinjen sparades. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


Ställer in en TimephasedDataCollection-instans för detta objekt. De tidsfasade data som är associerade med uppgiftsbaslinjen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | en TimephasedDataCollection-instans för detta objekt. |

