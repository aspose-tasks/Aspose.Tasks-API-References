---
title: WorkingTime
second_title: Aspose.Tasks for Java API Reference
description: Represents a working time during a weekday.
type: docs
weight: 362
url: /java/com.aspose.tasks/workingtime/
---

**Inheritance:**
java.lang.Object
```
public class WorkingTime
```

Represents a working time during a weekday.
## Constructors

| Constructor | Description |
| --- | --- |
| [WorkingTime(Date fromTime, Date toTime)](#WorkingTime-java.util.Date-java.util.Date-) | Initializes a new instance of the [WorkingTime](../../com.aspose.tasks/workingtime) class with a interval with the specified start and finish times. |
| [WorkingTime(double fromTime, double toTime)](#WorkingTime-double-double-) | Initializes a new instance of the [WorkingTime](../../com.aspose.tasks/workingtime) class with an interval item with the specified start and finish times. |
| [WorkingTime(int fromHours, int toHours)](#WorkingTime-int-int-) | Initializes a new instance of the [WorkingTime](../../com.aspose.tasks/workingtime) class with an interval item with the specified start and finish times. |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | Checks that the objects are equal. |
| [getFrom()](#getFrom--) | Gets the beginning of a working time. |
| [getTo()](#getTo--) | Gets the end of a working time. |
| [hashCode()](#hashCode--) | Returns a hash code value for the instance of the [WorkingTime](../../com.aspose.tasks/workingtime) class. |
### WorkingTime(Date fromTime, Date toTime) {#WorkingTime-java.util.Date-java.util.Date-}
```
public WorkingTime(Date fromTime, Date toTime)
```


Initializes a new instance of the [WorkingTime](../../com.aspose.tasks/workingtime) class with a interval with the specified start and finish times.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fromTime | java.util.Date | interval start time |
| toTime | java.util.Date | interval end time |

### WorkingTime(double fromTime, double toTime) {#WorkingTime-double-double-}
```
public WorkingTime(double fromTime, double toTime)
```


Initializes a new instance of the [WorkingTime](../../com.aspose.tasks/workingtime) class with an interval item with the specified start and finish times.

--------------------

&gt; ```
&gt; The overload of WorkingTime ctor can be used to initialize interval's start and end using TimeSpans:
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
| Parameter | Type | Description |
| --- | --- | --- |
| fromHours | int | Interval's start time represented by whole number of hours (0-24). |
| toHours | int | Interval's end time represented by whole number of hours (0-24). |

### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Checks that the objects are equal.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | Second object to compare. |

**Returns:**
boolean - True if the objects are equal, false otherwise.
### getFrom() {#getFrom--}
```
public final Date getFrom()
```


Gets the beginning of a working time.

**Returns:**
java.util.Date - the beginning of a working time.
### getTo() {#getTo--}
```
public final Date getTo()
```


Gets the end of a working time.

**Returns:**
java.util.Date - the end of a working time.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Returns a hash code value for the instance of the [WorkingTime](../../com.aspose.tasks/workingtime) class.

**Returns:**
int - returns a hash code value for this object.
