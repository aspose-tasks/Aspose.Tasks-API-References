---
title: "WorkingTime"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een werktijd tijdens een weekdag voor."
type: docs
weight: 365
url: /nl/java/com.aspose.tasks/workingtime/
---

**Inheritance:**
java.lang.Object
```
public class WorkingTime
```

Stelt een werktijd tijdens een weekdag voor.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [WorkingTime(Date fromTime, Date toTime)](#WorkingTime-java.util.Date-java.util.Date-) | Initialiseert een nieuw exemplaar van de [WorkingTime](../../com.aspose.tasks/workingtime) klasse met een interval met de opgegeven start- en eindtijden. |
| [WorkingTime(double fromTime, double toTime)](#WorkingTime-double-double-) | Initialiseert een nieuw exemplaar van de [WorkingTime](../../com.aspose.tasks/workingtime) klasse met een intervalitem met de opgegeven start- en eindtijden. |
| [WorkingTime(int fromHours, int toHours)](#WorkingTime-int-int-) | Initialiseert een nieuw exemplaar van de [WorkingTime](../../com.aspose.tasks/workingtime) klasse met een intervalitem met de opgegeven start- en eindtijden. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | Controleert of de objecten gelijk zijn. |
| [getFrom()](#getFrom--) | Haalt het begin van een werktijd op. |
| [getTo()](#getTo--) | Haalt het einde van een werktijd op. |
| [hashCode()](#hashCode--) | Retourneert een hashcode-waarde voor het exemplaar van de [WorkingTime](../../com.aspose.tasks/workingtime) klasse. |
### WorkingTime(Date fromTime, Date toTime) {#WorkingTime-java.util.Date-java.util.Date-}
```
public WorkingTime(Date fromTime, Date toTime)
```


Initialiseert een nieuw exemplaar van de [WorkingTime](../../com.aspose.tasks/workingtime) klasse met een interval met de opgegeven start- en eindtijden.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fromTime | java.util.Date | interval starttijd |
| toTime | java.util.Date | interval eindtijd |

### WorkingTime(double fromTime, double toTime) {#WorkingTime-double-double-}
```
public WorkingTime(double fromTime, double toTime)
```


Initialiseert een nieuw exemplaar van de [WorkingTime](../../com.aspose.tasks/workingtime) klasse met een intervalitem met de opgegeven start- en eindtijden.

--------------------

&gt; ```
&gt; De overload van de WorkingTime ctor kan worden gebruikt om de start en einde van het interval te initialiseren met TimeSpans:
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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fromHours | int | Starttijd van het interval weergegeven als een geheel aantal uren (0-24). |
| toHours | int | Eindtijd van het interval weergegeven als een geheel aantal uren (0-24). |

### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Controleert of de objecten gelijk zijn.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| obj | java.lang.Object | Tweede object om te vergelijken. |

**Returns:**
boolean - Waar als de objecten gelijk zijn, onwaar anders.
### getFrom() {#getFrom--}
```
public final Date getFrom()
```


Haalt het begin van een werktijd op.

**Returns:**
java.util.Date - het begin van een werktijd.
### getTo() {#getTo--}
```
public final Date getTo()
```


Haalt het einde van een werktijd op.

**Returns:**
java.util.Date - het einde van een werktijd.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Retourneert een hashcode-waarde voor het exemplaar van de [WorkingTime](../../com.aspose.tasks/workingtime) klasse.

**Returns:**
int - retourneert een hashcode-waarde voor dit object.
