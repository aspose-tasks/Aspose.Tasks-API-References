---
title: "TaskBaseline"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt de basislijn van een taak voor."
type: docs
weight: 291
url: /nl/java/com.aspose.tasks/taskbaseline/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.Baseline](../../com.aspose.tasks/baseline)

**All Implemented Interfaces:**
java.lang.Comparable
```
public class TaskBaseline extends Baseline implements Comparable<Baseline>
```

Stelt de basislijn van een taak voor.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [TaskBaseline(Task task)](#TaskBaseline-com.aspose.tasks.Task-) | Initialiseert een nieuw exemplaar van de [TaskBaseline](../../com.aspose.tasks/taskbaseline) klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [compareTo(TaskBaseline other)](#compareTo-com.aspose.tasks.TaskBaseline-) | IComparable interface-implementatie. |
| [equals(TaskBaseline other)](#equals-com.aspose.tasks.TaskBaseline-) | Retourneert een waarde die aangeeft of dit exemplaar gelijk is aan het opgegeven TaskBaseline-object. |
| [equals(Object obj)](#equals-java.lang.Object-) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| [getDuration()](#getDuration--) | Haalt de geplande duur van de taak op toen de basislijn werd opgeslagen. |
| [getEstimatedDuration()](#getEstimatedDuration--) | Haalt een waarde op die aangeeft of de basislijnduur van de taak geschat was. |
| [getFinish()](#getFinish--) | Haalt de geplande einddatum van de taak op toen de basislijn werd opgeslagen. |
| [getFixedCost()](#getFixedCost--) | Haalt een vaste kostprijs van de taak op toen de basislijn werd opgeslagen. |
| [getInterim()](#getInterim--) | Haalt een waarde op die aangeeft of dit een tussentijdse basislijn is. |
| [getStart()](#getStart--) | Haalt de geplande startdatum van de taak op toen de basislijn werd opgeslagen. |
| [getTimephasedData()](#getTimephasedData--) | Haalt een TimephasedDataCollection exemplaar op voor dit object. |
| [hashCode()](#hashCode--) | Retourneert een hashcodewaarde voor het exemplaar van de [TaskBaseline](../../com.aspose.tasks/taskbaseline) klasse. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Stelt de geplande duur van de taak in toen de basislijn werd opgeslagen. |
| [setEstimatedDuration(boolean value)](#setEstimatedDuration-boolean-) | Stelt een waarde in die aangeeft of de basislijnduur van de taak geschat was. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Stelt de geplande einddatum van de taak in toen de basislijn werd opgeslagen. |
| [setFixedCost(double value)](#setFixedCost-double-) | Stelt een vaste kost van de taak in wanneer de basislijn is opgeslagen. |
| [setInterim(boolean value)](#setInterim-boolean-) | Stelt een waarde in die aangeeft of dit een tussentijdse basislijn is. |
| [setStart(Date value)](#setStart-java.util.Date-) | Stelt de geplande startdatum van de taak in wanneer de basislijn is opgeslagen. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | Stelt een TimephasedDataCollection‑instantie in voor dit object. |
### TaskBaseline(Task task) {#TaskBaseline-com.aspose.tasks.Task-}
```
public TaskBaseline(Task task)
```


Initialiseert een nieuw exemplaar van de [TaskBaseline](../../com.aspose.tasks/taskbaseline) klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Bovenliggende taak van de basislijn. |

### compareTo(TaskBaseline other) {#compareTo-com.aspose.tasks.TaskBaseline-}
```
public final int compareTo(TaskBaseline other)
```


IComparable interface-implementatie. Vergelijkt deze instantie met het opgegeven Baseline-object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| other | [TaskBaseline](../../com.aspose.tasks/taskbaseline) | het opgegeven Baseline-object om deze instantie mee te vergelijken. |

**Returns:**
int - retourneert -1 als deze instantie kleiner is dan het opgegeven object, 1 als deze instantie groter is dan het opgegeven object; retourneert anders 0
### equals(TaskBaseline other) {#equals-com.aspose.tasks.TaskBaseline-}
```
public final boolean equals(TaskBaseline other)
```


Retourneert een waarde die aangeeft of dit exemplaar gelijk is aan het opgegeven TaskBaseline-object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| other | [TaskBaseline](../../com.aspose.tasks/taskbaseline) | het opgegeven AssignmentBaseline-object om te vergelijken met deze instantie. |

**Returns:**
boolean - retourneert true als deze instantie gelijk is aan het opgegeven TaskBaseline‑object; anders false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| obj | java.lang.Object | Het object om te vergelijken met deze instantie. |

**Returns:**
boolean - **True** als het opgegeven object een TaskBaseline is die dezelfde UID‑waarde heeft als deze instantie; anders **false**.
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Haalt de geplande duur van de taak op toen de basislijn werd opgeslagen.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the scheduled duration of the task when the baseline was saved.
### getEstimatedDuration() {#getEstimatedDuration--}
```
public final boolean getEstimatedDuration()
```


Haalt een waarde op die aangeeft of de basislijnduur van de taak geschat was.

**Returns:**
boolean - een waarde die aangeeft of de duur van de basislijn van de taak geschat was.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Haalt de geplande einddatum van de taak op toen de basislijn werd opgeslagen.

**Returns:**
java.util.Date - de geplande einddatum van de taak wanneer de basislijn is opgeslagen.
### getFixedCost() {#getFixedCost--}
```
public final double getFixedCost()
```


Haalt een vaste kostprijs van de taak op toen de basislijn werd opgeslagen.

**Returns:**
double - een vaste kost van de taak wanneer de basislijn is opgeslagen.
### getInterim() {#getInterim--}
```
public final boolean getInterim()
```


Haalt een waarde op die aangeeft of dit een tussentijdse basislijn is.

**Returns:**
boolean - een waarde die aangeeft of dit een tussentijdse basislijn is.
### getStart() {#getStart--}
```
public final Date getStart()
```


Haalt de geplande startdatum van de taak op toen de basislijn werd opgeslagen.

**Returns:**
java.util.Date - de geplande startdatum van de taak wanneer de basislijn is opgeslagen.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


Haalt een TimephasedDataCollection‑instantie op voor dit object. De tijdgephaseerde gegevens die gekoppeld zijn aan de taakbasislijn.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - a TimephasedDataCollection instance for this object.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Retourneert een hashcodewaarde voor het exemplaar van de [TaskBaseline](../../com.aspose.tasks/taskbaseline) klasse.

**Returns:**
int - retourneert een hashcode-waarde voor dit object.
### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Stelt de geplande duur van de taak in toen de basislijn werd opgeslagen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | de geplande duur van de taak wanneer de basislijn is opgeslagen. |

### setEstimatedDuration(boolean value) {#setEstimatedDuration-boolean-}
```
public final void setEstimatedDuration(boolean value)
```


Stelt een waarde in die aangeeft of de basislijnduur van de taak geschat was.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of de duur van de basislijn van de taak geschat was. |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Stelt de geplande einddatum van de taak in toen de basislijn werd opgeslagen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date | de geplande einddatum van de taak wanneer de basislijn is opgeslagen. |

### setFixedCost(double value) {#setFixedCost-double-}
```
public final void setFixedCost(double value)
```


Stelt een vaste kost van de taak in wanneer de basislijn is opgeslagen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | double | een vaste kost van de taak wanneer de basislijn is opgeslagen. |

### setInterim(boolean value) {#setInterim-boolean-}
```
public final void setInterim(boolean value)
```


Stelt een waarde in die aangeeft of dit een tussentijdse basislijn is.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of dit een tussentijdse basislijn is. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Stelt de geplande startdatum van de taak in wanneer de basislijn is opgeslagen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date | de geplande startdatum van de taak wanneer de basislijn is opgeslagen. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


Stelt een TimephasedDataCollection‑instantie in voor dit object. De tijdgephaseerde gegevens die gekoppeld zijn aan de taakbasislijn.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | een TimephasedDataCollection‑instantie voor dit object. |

