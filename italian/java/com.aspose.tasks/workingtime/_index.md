---
title: "WorkingTime"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta un orario di lavoro durante un giorno della settimana."
type: docs
weight: 365
url: /it/java/com.aspose.tasks/workingtime/
---

**Inheritance:**
java.lang.Object
```
public class WorkingTime
```

Rappresenta un orario di lavoro durante un giorno della settimana.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [WorkingTime(Date fromTime, Date toTime)](#WorkingTime-java.util.Date-java.util.Date-) | Inizializza una nuova istanza della classe [WorkingTime](../../com.aspose.tasks/workingtime) con un intervallo con gli orari di inizio e fine specificati. |
| [WorkingTime(double fromTime, double toTime)](#WorkingTime-double-double-) | Inizializza una nuova istanza della classe [WorkingTime](../../com.aspose.tasks/workingtime) con un elemento di intervallo con gli orari di inizio e fine specificati. |
| [WorkingTime(int fromHours, int toHours)](#WorkingTime-int-int-) | Inizializza una nuova istanza della classe [WorkingTime](../../com.aspose.tasks/workingtime) con un elemento di intervallo con gli orari di inizio e fine specificati. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | Verifica che gli oggetti siano uguali. |
| [getFrom()](#getFrom--) | Ottiene l'inizio di un orario di lavoro. |
| [getTo()](#getTo--) | Ottiene la fine di un orario di lavoro. |
| [hashCode()](#hashCode--) | Restituisce un valore di hash code per l'istanza della classe [WorkingTime](../../com.aspose.tasks/workingtime). |
### WorkingTime(Date fromTime, Date toTime) {#WorkingTime-java.util.Date-java.util.Date-}
```
public WorkingTime(Date fromTime, Date toTime)
```


Inizializza una nuova istanza della classe [WorkingTime](../../com.aspose.tasks/workingtime) con un intervallo con gli orari di inizio e fine specificati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fromTime | java.util.Date | orario di inizio dell'intervallo |
| toTime | java.util.Date | orario di fine dell'intervallo |

### WorkingTime(double fromTime, double toTime) {#WorkingTime-double-double-}
```
public WorkingTime(double fromTime, double toTime)
```


Inizializza una nuova istanza della classe [WorkingTime](../../com.aspose.tasks/workingtime) con un elemento di intervallo con gli orari di inizio e fine specificati.

--------------------

&gt; ```
&gt; La sovraccarico del costruttore WorkingTime può essere usata per inizializzare l'inizio e la fine dell'intervallo usando i TimeSpans:
&gt; ``````

 [C#]
var wt = new WorkingTime(new TimeSpan(9, 0, 0), new TimeSpan(18, 0, 0));
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fromTime | double | Interval's start time represented by double struct. |
| toTime | double | Interval's end time represented by double struct. |

### WorkingTime(int fromHours, int toHours) {#WorkingTime-int-int-}
```
public WorkingTime(int fromHours, int toHours)
```


Initializes a new instance of the [WorkingTime](../../com.aspose.tasks/workingtime) class with an interval item with the specified start and finish times.

--------------------

&gt; ```
&gt; The overload of WorkingTime ctor can be used to initialize interval's start and end using whole hours:
&gt; ``````

 [C#]
 var wt = new WorkingTime(9, 13);
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fromHours | int | L'orario di inizio dell'intervallo è rappresentato da un numero intero di ore (0-24). |
| toHours | int | L'orario di fine dell'intervallo è rappresentato da un numero intero di ore (0-24). |

### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Verifica che gli oggetti siano uguali.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | java.lang.Object | Secondo oggetto da confrontare. |

**Returns:**
boolean - True se gli oggetti sono uguali, false altrimenti.
### getFrom() {#getFrom--}
```
public final Date getFrom()
```


Ottiene l'inizio di un orario di lavoro.

**Returns:**
java.util.Date - l'inizio di un orario di lavoro.
### getTo() {#getTo--}
```
public final Date getTo()
```


Ottiene la fine di un orario di lavoro.

**Returns:**
java.util.Date - la fine di un orario di lavoro.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Restituisce un valore di hash code per l'istanza della classe [WorkingTime](../../com.aspose.tasks/workingtime).

**Returns:**
int - restituisce un valore di codice hash per questo oggetto.
