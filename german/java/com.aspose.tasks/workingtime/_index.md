---
title: "WorkingTime"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt eine Arbeitszeit während eines Wochentags dar."
type: docs
weight: 365
url: /de/java/com.aspose.tasks/workingtime/
---

**Inheritance:**
java.lang.Object
```
public class WorkingTime
```

Stellt eine Arbeitszeit während eines Wochentags dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [WorkingTime(Date fromTime, Date toTime)](#WorkingTime-java.util.Date-java.util.Date-) | Initialisiert eine neue Instanz der [WorkingTime](../../com.aspose.tasks/workingtime)-Klasse mit einem Intervall mit den angegebenen Start- und Endzeiten. |
| [WorkingTime(double fromTime, double toTime)](#WorkingTime-double-double-) | Initialisiert eine neue Instanz der [WorkingTime](../../com.aspose.tasks/workingtime)-Klasse mit einem Intervall-Element mit den angegebenen Start- und Endzeiten. |
| [WorkingTime(int fromHours, int toHours)](#WorkingTime-int-int-) | Initialisiert eine neue Instanz der [WorkingTime](../../com.aspose.tasks/workingtime)-Klasse mit einem Intervall-Element mit den angegebenen Start- und Endzeiten. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | Überprüft, ob die Objekte gleich sind. |
| [getFrom()](#getFrom--) | Gibt den Beginn einer Arbeitszeit zurück. |
| [getTo()](#getTo--) | Gibt das Ende einer Arbeitszeit zurück. |
| [hashCode()](#hashCode--) | Gibt einen Hashcode-Wert für die Instanz der [WorkingTime](../../com.aspose.tasks/workingtime)-Klasse zurück. |
### WorkingTime(Date fromTime, Date toTime) {#WorkingTime-java.util.Date-java.util.Date-}
```
public WorkingTime(Date fromTime, Date toTime)
```


Initialisiert eine neue Instanz der [WorkingTime](../../com.aspose.tasks/workingtime)-Klasse mit einem Intervall mit den angegebenen Start- und Endzeiten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fromTime | java.util.Date | Intervall-Startzeit |
| toTime | java.util.Date | Intervall-Endzeit |

### WorkingTime(double fromTime, double toTime) {#WorkingTime-double-double-}
```
public WorkingTime(double fromTime, double toTime)
```


Initialisiert eine neue Instanz der [WorkingTime](../../com.aspose.tasks/workingtime)-Klasse mit einem Intervall-Element mit den angegebenen Start- und Endzeiten.

--------------------

&gt; ```
&gt; Die Überladung des WorkingTime ctor kann verwendet werden, um den Start und das Ende des Intervalls mit TimeSpans zu initialisieren:
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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fromHours | int | Startzeit des Intervalls, dargestellt als ganze Stundenzahl (0‑24). |
| toHours | int | Endzeit des Intervalls, dargestellt als ganze Stundenzahl (0‑24). |

### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Überprüft, ob die Objekte gleich sind.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | java.lang.Object | Zweites Objekt zum Vergleichen. |

**Returns:**
boolean - True, wenn die Objekte gleich sind, sonst false.
### getFrom() {#getFrom--}
```
public final Date getFrom()
```


Gibt den Beginn einer Arbeitszeit zurück.

**Returns:**
java.util.Date - der Beginn einer Arbeitszeit.
### getTo() {#getTo--}
```
public final Date getTo()
```


Gibt das Ende einer Arbeitszeit zurück.

**Returns:**
java.util.Date - das Ende einer Arbeitszeit.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Gibt einen Hashcode-Wert für die Instanz der [WorkingTime](../../com.aspose.tasks/workingtime)-Klasse zurück.

**Returns:**
int - gibt einen Hashcode-Wert für dieses Objekt zurück.
