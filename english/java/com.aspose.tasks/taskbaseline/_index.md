---
title: TaskBaseline
second_title: Aspose.Tasks for Java API Reference
description: Represents Baseline of a Task.
type: docs
weight: 290
url: /java/com.aspose.tasks/taskbaseline/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.Baseline](../../com.aspose.tasks/baseline)

**All Implemented Interfaces:**
java.lang.Comparable
```
public class TaskBaseline extends Baseline implements Comparable<Baseline>
```

Represents Baseline of a Task.
## Constructors

| Constructor | Description |
| --- | --- |
| [TaskBaseline(Task task)](#TaskBaseline-com.aspose.tasks.Task-) | Initializes a new instance of the [TaskBaseline](../../com.aspose.tasks/taskbaseline) class. |
## Methods

| Method | Description |
| --- | --- |
| [compareTo(TaskBaseline other)](#compareTo-com.aspose.tasks.TaskBaseline-) | IComparable interface implementation. |
| [equals(TaskBaseline other)](#equals-com.aspose.tasks.TaskBaseline-) | Returns a value indicating whether this instance is equal to the specified TaskBaseline object. |
| [equals(Object obj)](#equals-java.lang.Object-) | Returns a value indicating whether this instance is equal to a specified object. |
| [getDuration()](#getDuration--) | Gets the scheduled duration of the task when the baseline was saved. |
| [getEstimatedDuration()](#getEstimatedDuration--) | Gets a value indicating whether the baseline duration of the task was estimated. |
| [getFinish()](#getFinish--) | Gets the scheduled finish date of the task when the baseline was saved. |
| [getFixedCost()](#getFixedCost--) | Gets a fixed cost of the task when the baseline was saved. |
| [getInterim()](#getInterim--) | Gets a value indicating whether this is an Interim Baseline. |
| [getStart()](#getStart--) | Gets the scheduled start date of the task when the baseline was saved. |
| [getTimephasedData()](#getTimephasedData--) | Gets a TimephasedDataCollection instance for this object. |
| [hashCode()](#hashCode--) | Returns a hash code value for the instance of the [TaskBaseline](../../com.aspose.tasks/taskbaseline) class. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Sets the scheduled duration of the task when the baseline was saved. |
| [setEstimatedDuration(boolean value)](#setEstimatedDuration-boolean-) | Sets a value indicating whether the baseline duration of the task was estimated. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Sets the scheduled finish date of the task when the baseline was saved. |
| [setFixedCost(double value)](#setFixedCost-double-) | Sets a fixed cost of the task when the baseline was saved. |
| [setInterim(boolean value)](#setInterim-boolean-) | Sets a value indicating whether this is an Interim Baseline. |
| [setStart(Date value)](#setStart-java.util.Date-) | Sets the scheduled start date of the task when the baseline was saved. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | Sets a TimephasedDataCollection instance for this object. |
### TaskBaseline(Task task) {#TaskBaseline-com.aspose.tasks.Task-}
```
public TaskBaseline(Task task)
```


Initializes a new instance of the [TaskBaseline](../../com.aspose.tasks/taskbaseline) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Baseline's parent task. |

### compareTo(TaskBaseline other) {#compareTo-com.aspose.tasks.TaskBaseline-}
```
public final int compareTo(TaskBaseline other)
```


IComparable interface implementation. Compares this instance to the specified Baseline object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| other | [TaskBaseline](../../com.aspose.tasks/taskbaseline) | the specified Baseline object to compare this instance to. |

**Returns:**
int - returns -1 if this instance is less than the specified object, 1 if this instance is greater than the specified object; otherwise returns 0
### equals(TaskBaseline other) {#equals-com.aspose.tasks.TaskBaseline-}
```
public final boolean equals(TaskBaseline other)
```


Returns a value indicating whether this instance is equal to the specified TaskBaseline object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| other | [TaskBaseline](../../com.aspose.tasks/taskbaseline) | the specified AssignmentBaseline object to compare with this instance. |

**Returns:**
boolean - returns true if this instance is equal to the specified TaskBaseline object; otherwise, false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Returns a value indicating whether this instance is equal to a specified object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | The object to compare with this instance. |

**Returns:**
boolean - **True** if the specified object is a TaskBaseline that has the same UID value as this instance; otherwise, **false**.
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Gets the scheduled duration of the task when the baseline was saved.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the scheduled duration of the task when the baseline was saved.
### getEstimatedDuration() {#getEstimatedDuration--}
```
public final boolean getEstimatedDuration()
```


Gets a value indicating whether the baseline duration of the task was estimated.

**Returns:**
boolean - a value indicating whether the baseline duration of the task was estimated.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Gets the scheduled finish date of the task when the baseline was saved.

**Returns:**
java.util.Date - the scheduled finish date of the task when the baseline was saved.
### getFixedCost() {#getFixedCost--}
```
public final double getFixedCost()
```


Gets a fixed cost of the task when the baseline was saved.

**Returns:**
double - a fixed cost of the task when the baseline was saved.
### getInterim() {#getInterim--}
```
public final boolean getInterim()
```


Gets a value indicating whether this is an Interim Baseline.

**Returns:**
boolean - a value indicating whether this is an Interim Baseline.
### getStart() {#getStart--}
```
public final Date getStart()
```


Gets the scheduled start date of the task when the baseline was saved.

**Returns:**
java.util.Date - the scheduled start date of the task when the baseline was saved.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


Gets a TimephasedDataCollection instance for this object. The time phased data associated with the task baseline.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - a TimephasedDataCollection instance for this object.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Returns a hash code value for the instance of the [TaskBaseline](../../com.aspose.tasks/taskbaseline) class.

**Returns:**
int - returns a hash code value for this object.
### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Sets the scheduled duration of the task when the baseline was saved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | the scheduled duration of the task when the baseline was saved. |

### setEstimatedDuration(boolean value) {#setEstimatedDuration-boolean-}
```
public final void setEstimatedDuration(boolean value)
```


Sets a value indicating whether the baseline duration of the task was estimated.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether the baseline duration of the task was estimated. |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Sets the scheduled finish date of the task when the baseline was saved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | the scheduled finish date of the task when the baseline was saved. |

### setFixedCost(double value) {#setFixedCost-double-}
```
public final void setFixedCost(double value)
```


Sets a fixed cost of the task when the baseline was saved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a fixed cost of the task when the baseline was saved. |

### setInterim(boolean value) {#setInterim-boolean-}
```
public final void setInterim(boolean value)
```


Sets a value indicating whether this is an Interim Baseline.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether this is an Interim Baseline. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Sets the scheduled start date of the task when the baseline was saved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | the scheduled start date of the task when the baseline was saved. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


Sets a TimephasedDataCollection instance for this object. The time phased data associated with the task baseline.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | a TimephasedDataCollection instance for this object. |

