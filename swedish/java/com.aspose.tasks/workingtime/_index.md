---
title: "WorkingTime"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar en arbetstid under en veckodag."
type: docs
weight: 365
url: /sv/java/com.aspose.tasks/workingtime/
---

**Inheritance:**
java.lang.Object
```
public class WorkingTime
```

Representerar en arbetstid under en veckodag.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [WorkingTime(Date fromTime, Date toTime)](#WorkingTime-java.util.Date-java.util.Date-) | Initierar en ny instans av klassen [WorkingTime](../../com.aspose.tasks/workingtime) med ett intervall med de angivna start- och sluttiderna. |
| [WorkingTime(double fromTime, double toTime)](#WorkingTime-double-double-) | Initierar en ny instans av klassen [WorkingTime](../../com.aspose.tasks/workingtime) med ett intervallselement med de angivna start- och sluttiderna. |
| [WorkingTime(int fromHours, int toHours)](#WorkingTime-int-int-) | Initierar en ny instans av klassen [WorkingTime](../../com.aspose.tasks/workingtime) med ett intervallselement med de angivna start- och sluttiderna. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | Kontrollerar att objekten är lika. |
| [getFrom()](#getFrom--) | Hämtar början av en arbetstid. |
| [getTo()](#getTo--) | Hämtar slutet av en arbetstid. |
| [hashCode()](#hashCode--) | Returnerar ett hashkodvärde för instansen av klassen [WorkingTime](../../com.aspose.tasks/workingtime). |
### WorkingTime(Date fromTime, Date toTime) {#WorkingTime-java.util.Date-java.util.Date-}
```
public WorkingTime(Date fromTime, Date toTime)
```


Initierar en ny instans av klassen [WorkingTime](../../com.aspose.tasks/workingtime) med ett intervall med de angivna start- och sluttiderna.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fromTime | java.util.Date | intervallens starttid |
| toTime | java.util.Date | intervallens sluttid |

### WorkingTime(double fromTime, double toTime) {#WorkingTime-double-double-}
```
public WorkingTime(double fromTime, double toTime)
```


Initierar en ny instans av klassen [WorkingTime](../../com.aspose.tasks/workingtime) med ett intervallselement med de angivna start- och sluttiderna.

--------------------

&gt; ```
&gt; Överlagringen av WorkingTime ctor kan användas för att initiera intervallets start och slut med TimeSpans:
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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fromHours | int | Intervallets starttid representerad av ett helt antal timmar (0-24). |
| toHours | int | Intervallets sluttid representerad av ett helt antal timmar (0-24). |

### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Kontrollerar att objekten är lika.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | java.lang.Object | Andra objektet att jämföra. |

**Returns:**
boolean - Sant om objekten är lika, falskt annars.
### getFrom() {#getFrom--}
```
public final Date getFrom()
```


Hämtar början av en arbetstid.

**Returns:**
java.util.Date - början av en arbetstid.
### getTo() {#getTo--}
```
public final Date getTo()
```


Hämtar slutet av en arbetstid.

**Returns:**
java.util.Date - slutet av en arbetstid.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Returnerar ett hashkodvärde för instansen av klassen [WorkingTime](../../com.aspose.tasks/workingtime).

**Returns:**
int - returnerar ett hash‑kodvärde för detta objekt.
