---
title: "TaskBaseline"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta la baseline di un'attività."
type: docs
weight: 291
url: /it/java/com.aspose.tasks/taskbaseline/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.Baseline](../../com.aspose.tasks/baseline)

**All Implemented Interfaces:**
java.lang.Comparable
```
public class TaskBaseline extends Baseline implements Comparable<Baseline>
```

Rappresenta la baseline di un'attività.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [TaskBaseline(Task task)](#TaskBaseline-com.aspose.tasks.Task-) | Inizializza una nuova istanza della classe [TaskBaseline](../../com.aspose.tasks/taskbaseline). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [compareTo(TaskBaseline other)](#compareTo-com.aspose.tasks.TaskBaseline-) | Implementazione dell'interfaccia IComparable. |
| [equals(TaskBaseline other)](#equals-com.aspose.tasks.TaskBaseline-) | Restituisce un valore che indica se questa istanza è uguale all'oggetto TaskBaseline specificato. |
| [equals(Object obj)](#equals-java.lang.Object-) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| [getDuration()](#getDuration--) | Ottiene la durata programmata dell'attività quando la baseline è stata salvata. |
| [getEstimatedDuration()](#getEstimatedDuration--) | Ottiene un valore che indica se la durata della baseline dell'attività era stimata. |
| [getFinish()](#getFinish--) | Ottiene la data di fine programmata dell'attività quando la baseline è stata salvata. |
| [getFixedCost()](#getFixedCost--) | Ottiene un costo fisso dell'attività quando la baseline è stata salvata. |
| [getInterim()](#getInterim--) | Ottiene un valore che indica se questa è una Baseline intermedia. |
| [getStart()](#getStart--) | Ottiene la data di inizio programmata dell'attività quando la baseline è stata salvata. |
| [getTimephasedData()](#getTimephasedData--) | Ottiene un'istanza di TimephasedDataCollection per questo oggetto. |
| [hashCode()](#hashCode--) | Restituisce un valore di codice hash per l'istanza della classe [TaskBaseline](../../com.aspose.tasks/taskbaseline). |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Imposta la durata programmata dell'attività quando la baseline è stata salvata. |
| [setEstimatedDuration(boolean value)](#setEstimatedDuration-boolean-) | Imposta un valore che indica se la durata della baseline dell'attività era stimata. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Imposta la data di fine programmata dell'attività quando la baseline è stata salvata. |
| [setFixedCost(double value)](#setFixedCost-double-) | Imposta un costo fisso dell'attività quando la baseline è stata salvata. |
| [setInterim(boolean value)](#setInterim-boolean-) | Imposta un valore che indica se questa è una Interim Baseline. |
| [setStart(Date value)](#setStart-java.util.Date-) | Imposta la data di inizio programmata dell'attività quando la baseline è stata salvata. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | Imposta un'istanza di TimephasedDataCollection per questo oggetto. |
### TaskBaseline(Task task) {#TaskBaseline-com.aspose.tasks.Task-}
```
public TaskBaseline(Task task)
```


Inizializza una nuova istanza della classe [TaskBaseline](../../com.aspose.tasks/taskbaseline).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Attività padre della baseline. |

### compareTo(TaskBaseline other) {#compareTo-com.aspose.tasks.TaskBaseline-}
```
public final int compareTo(TaskBaseline other)
```


Implementazione dell'interfaccia IComparable. Confronta questa istanza con l'oggetto Baseline specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| other | [TaskBaseline](../../com.aspose.tasks/taskbaseline) | l'oggetto Baseline specificato con cui confrontare questa istanza. |

**Returns:**
int - restituisce -1 se questa istanza è inferiore all'oggetto specificato, 1 se questa istanza è superiore all'oggetto specificato; altrimenti restituisce 0
### equals(TaskBaseline other) {#equals-com.aspose.tasks.TaskBaseline-}
```
public final boolean equals(TaskBaseline other)
```


Restituisce un valore che indica se questa istanza è uguale all'oggetto TaskBaseline specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| other | [TaskBaseline](../../com.aspose.tasks/taskbaseline) | l'oggetto AssignmentBaseline specificato da confrontare con questa istanza. |

**Returns:**
boolean - restituisce true se questa istanza è uguale all'oggetto TaskBaseline specificato; altrimenti, false.
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
boolean - **True** se l'oggetto specificato è un TaskBaseline che ha lo stesso valore UID di questa istanza; altrimenti, **false**.
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Ottiene la durata programmata dell'attività quando la baseline è stata salvata.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the scheduled duration of the task when the baseline was saved.
### getEstimatedDuration() {#getEstimatedDuration--}
```
public final boolean getEstimatedDuration()
```


Ottiene un valore che indica se la durata della baseline dell'attività era stimata.

**Returns:**
boolean - un valore che indica se la durata della baseline dell'attività era stimata.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Ottiene la data di fine programmata dell'attività quando la baseline è stata salvata.

**Returns:**
java.util.Date - la data di fine programmata dell'attività quando la baseline è stata salvata.
### getFixedCost() {#getFixedCost--}
```
public final double getFixedCost()
```


Ottiene un costo fisso dell'attività quando la baseline è stata salvata.

**Returns:**
double - un costo fisso dell'attività quando la baseline è stata salvata.
### getInterim() {#getInterim--}
```
public final boolean getInterim()
```


Ottiene un valore che indica se questa è una Baseline intermedia.

**Returns:**
boolean - un valore che indica se questa è una Interim Baseline.
### getStart() {#getStart--}
```
public final Date getStart()
```


Ottiene la data di inizio programmata dell'attività quando la baseline è stata salvata.

**Returns:**
java.util.Date - la data di inizio programmata dell'attività quando la baseline è stata salvata.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


Ottiene un'istanza di TimephasedDataCollection per questo oggetto. I dati temporizzati associati alla baseline dell'attività.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - a TimephasedDataCollection instance for this object.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Restituisce un valore di codice hash per l'istanza della classe [TaskBaseline](../../com.aspose.tasks/taskbaseline).

**Returns:**
int - restituisce un valore di codice hash per questo oggetto.
### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Imposta la durata programmata dell'attività quando la baseline è stata salvata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | la durata programmata dell'attività quando la baseline è stata salvata. |

### setEstimatedDuration(boolean value) {#setEstimatedDuration-boolean-}
```
public final void setEstimatedDuration(boolean value)
```


Imposta un valore che indica se la durata della baseline dell'attività era stimata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se la durata della baseline dell'attività era stimata. |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Imposta la data di fine programmata dell'attività quando la baseline è stata salvata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date | la data di fine programmata dell'attività quando la baseline è stata salvata. |

### setFixedCost(double value) {#setFixedCost-double-}
```
public final void setFixedCost(double value)
```


Imposta un costo fisso dell'attività quando la baseline è stata salvata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double | un costo fisso dell'attività quando la baseline è stata salvata. |

### setInterim(boolean value) {#setInterim-boolean-}
```
public final void setInterim(boolean value)
```


Imposta un valore che indica se questa è una Interim Baseline.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se questa è una Interim Baseline. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Imposta la data di inizio programmata dell'attività quando la baseline è stata salvata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date | la data di inizio programmata dell'attività quando la baseline è stata salvata. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


Imposta un'istanza di TimephasedDataCollection per questo oggetto. I dati temporizzati associati alla baseline dell'attività.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | un'istanza di TimephasedDataCollection per questo oggetto. |

