---
title: "TaskLink"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta un collegamento predecessore."
type: docs
weight: 295
url: /it/java/com.aspose.tasks/tasklink/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable
```
public final class TaskLink implements System.IEquatable<TaskLink>
```

Rappresenta un collegamento predecessore.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(TaskLink other)](#equals-com.aspose.tasks.TaskLink-) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| [equals(Object obj)](#equals-java.lang.Object-) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| [getCrossProjectName()](#getCrossProjectName--) | Ottiene il progetto predecessore esterno. |
| [getLagFormat()](#getLagFormat--) | Ottiene il formato per esprimere il formato di ritardo. |
| [getLinkLag()](#getLinkLag--) | Ottiene il ritardo in decimi di minuto o in percentuale. |
| [getLinkLagTimeSpan()](#getLinkLagTimeSpan--) | Ottiene la durata del ritardo, a seconda di LagFormat. |
| [getLinkType()](#getLinkType--) | Ottiene il tipo di un collegamento. |
| [getPredTask()](#getPredTask--) | Ottiene l'attività predecessore. |
| [getSuccTask()](#getSuccTask--) | Ottiene l'attività successiva. |
| [hashCode()](#hashCode--) | Restituisce un valore di codice hash per l'istanza della classe [TaskLink](../../com.aspose.tasks/tasklink). |
| [isCrossProject()](#isCrossProject--) | Ottiene un valore che indica se un predecessore fa parte di un altro progetto. |
| [setCrossProject(boolean value)](#setCrossProject-boolean-) | Imposta un valore che indica se un predecessore fa parte di un altro progetto. |
| [setCrossProjectName(String value)](#setCrossProjectName-java.lang.String-) | Imposta il progetto predecessore esterno. |
| [setLagFormat(byte value)](#setLagFormat-byte-) | Imposta il formato per esprimere il formato di ritardo. |
| [setLinkLag(int value)](#setLinkLag-int-) | Imposta il ritardo in decimi di minuto o in percentuale. |
| [setLinkLagTimeSpan(double value)](#setLinkLagTimeSpan-double-) | Imposta la durata del ritardo, a seconda di LagFormat. |
| [setLinkType(int value)](#setLinkType-int-) | Imposta il tipo di un collegamento. |
| [setPredTask(Task value)](#setPredTask-com.aspose.tasks.Task-) | Imposta l'attività predecessore. |
| [setSuccTask(Task value)](#setSuccTask-com.aspose.tasks.Task-) | Imposta l'attività successiva. |
| [toString()](#toString--) | Restituisce la rappresentazione stringa di un TaskLink. |
### equals(TaskLink other) {#equals-com.aspose.tasks.TaskLink-}
```
public final boolean equals(TaskLink other)
```


Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| other | [TaskLink](../../com.aspose.tasks/tasklink) | L'istanza specificata della classe [TaskLink](../../com.aspose.tasks/tasklink) da confrontare con questa istanza. |

**Returns:**
boolean - **True** se l'istanza specificata della classe [TaskLink](../../com.aspose.tasks/tasklink) ha gli stessi compiti predecessori e successori di questa istanza; altrimenti, **false**.
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
boolean - **True** se l'oggetto specificato è un TaskLink che ha lo stesso predecessore e successore di questa istanza; altrimenti, **false**.
### getCrossProjectName() {#getCrossProjectName--}
```
public final String getCrossProjectName()
```


Ottiene il progetto predecessore esterno.

**Returns:**
java.lang.String - il progetto predecessore esterno.
### getLagFormat() {#getLagFormat--}
```
public final byte getLagFormat()
```


Ottiene il formato per esprimere il formato di ritardo.

**Returns:**
byte - il formato per esprimere il formato di ritardo.
### getLinkLag() {#getLinkLag--}
```
public final int getLinkLag()
```


Ottiene il ritardo in decimi di minuto o in percentuale.

**Returns:**
int - il ritardo in decimi di minuto o percentuale.
### getLinkLagTimeSpan() {#getLinkLagTimeSpan--}
```
public final double getLinkLagTimeSpan()
```


Ottiene la durata del ritardo, a seconda di LagFormat.

**Returns:**
double - durata del ritardo, a seconda di LagFormat.
### getLinkType() {#getLinkType--}
```
public final int getLinkType()
```


Ottiene il tipo di un collegamento.

**Returns:**
int - il tipo di un collegamento.
### getPredTask() {#getPredTask--}
```
public final Task getPredTask()
```


Ottiene l'attività predecessore.

**Returns:**
[Task](../../com.aspose.tasks/task) - the predecessor task.
### getSuccTask() {#getSuccTask--}
```
public final Task getSuccTask()
```


Ottiene l'attività successiva.

**Returns:**
[Task](../../com.aspose.tasks/task) - the successor task.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Restituisce un valore di codice hash per l'istanza della classe [TaskLink](../../com.aspose.tasks/tasklink).

**Returns:**
int - restituisce un valore di codice hash per questo oggetto.
### isCrossProject() {#isCrossProject--}
```
public final boolean isCrossProject()
```


Ottiene un valore che indica se un predecessore fa parte di un altro progetto.

**Returns:**
boolean - un valore che indica se un predecessore fa parte di un altro progetto.
### setCrossProject(boolean value) {#setCrossProject-boolean-}
```
public final void setCrossProject(boolean value)
```


Imposta un valore che indica se un predecessore fa parte di un altro progetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se un predecessore fa parte di un altro progetto. |

### setCrossProjectName(String value) {#setCrossProjectName-java.lang.String-}
```
public final void setCrossProjectName(String value)
```


Imposta il progetto predecessore esterno.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | il progetto predecessore esterno. |

### setLagFormat(byte value) {#setLagFormat-byte-}
```
public final void setLagFormat(byte value)
```


Imposta il formato per esprimere il formato di ritardo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | byte | il formato per esprimere il formato di ritardo. |

### setLinkLag(int value) {#setLinkLag-int-}
```
public final void setLinkLag(int value)
```


Imposta il ritardo in decimi di minuto o in percentuale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | il ritardo in decimi di minuto o percentuale. |

### setLinkLagTimeSpan(double value) {#setLinkLagTimeSpan-double-}
```
public final void setLinkLagTimeSpan(double value)
```


Imposta la durata del ritardo, a seconda di LagFormat.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double | durata del ritardo, a seconda di LagFormat. |

### setLinkType(int value) {#setLinkType-int-}
```
public final void setLinkType(int value)
```


Imposta il tipo di un collegamento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | il tipo di un collegamento. |

### setPredTask(Task value) {#setPredTask-com.aspose.tasks.Task-}
```
public final void setPredTask(Task value)
```


Imposta l'attività predecessore.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | l'attività predecessore. |

### setSuccTask(Task value) {#setSuccTask-com.aspose.tasks.Task-}
```
public final void setSuccTask(Task value)
```


Imposta l'attività successiva.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | l'attività successore. |

### toString() {#toString--}
```
public String toString()
```


Restituisce la rappresentazione stringa di un TaskLink. I dettagli esatti della rappresentazione non sono specificati e sono soggetti a modifiche.

**Returns:**
java.lang.String - stringa che rappresenta l'oggetto TaskLink.
