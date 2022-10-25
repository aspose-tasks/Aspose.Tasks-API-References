---
title: TaskLink
second_title: Aspose.Tasks for Java API Reference
description: Represents a predecessor link.
type: docs
weight: 269
url: /java/com.aspose.tasks/tasklink/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable
```
public class TaskLink implements System.IEquatable<TaskLink>
```

Represents a predecessor link.
## Methods

| Method | Description |
| --- | --- |
| [equals(TaskLink other)](#equals-com.aspose.tasks.TaskLink-) | Returns a value indicating whether this instance is equal to a specified object. |
| [equals(Object obj)](#equals-java.lang.Object-) | Returns a value indicating whether this instance is equal to a specified object. |
| [getCrossProjectName()](#getCrossProjectName--) | Gets the external predecessor project. |
| [setCrossProjectName(String value)](#setCrossProjectName-java.lang.String-) | Sets the external predecessor project. |
| [getLagFormat()](#getLagFormat--) | Gets the format for expressing the lag format. |
| [setLagFormat(int value)](#setLagFormat-int-) | Sets the format for expressing the lag format. |
| [getLinkLag()](#getLinkLag--) | Gets the amount of lag in tenths of a minute or percentage. |
| [setLinkLag(int value)](#setLinkLag-int-) | Sets the amount of lag in tenths of a minute or percentage. |
| [getLinkType()](#getLinkType--) | Gets the type of a link. |
| [setLinkType(int value)](#setLinkType-int-) | Sets the type of a link. |
| [getPredTask()](#getPredTask--) | Gets the predecessor task. |
| [setPredTask(Task value)](#setPredTask-com.aspose.tasks.Task-) | Sets the predecessor task. |
| [getSuccTask()](#getSuccTask--) | Gets the successor task. |
| [setSuccTask(Task value)](#setSuccTask-com.aspose.tasks.Task-) | Sets the successor task. |
| [hashCode()](#hashCode--) | Returns a hash code value for the instance of the [TaskLink](../../com.aspose.tasks/tasklink) class. |
| [isCrossProject()](#isCrossProject--) | Gets a value indicating whether a predecessor is part of another project. |
| [setCrossProject(boolean value)](#setCrossProject-boolean-) | Sets a value indicating whether a predecessor is part of another project. |
| [toString()](#toString--) | Returns string representation of a TaskLink. |
### equals(TaskLink other) {#equals-com.aspose.tasks.TaskLink-}
```
public final boolean equals(TaskLink other)
```


Returns a value indicating whether this instance is equal to a specified object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| other | [TaskLink](../../com.aspose.tasks/tasklink) | The specified instance of the [TaskLink](../../com.aspose.tasks/tasklink) class to compare with this instance. |

**Returns:**
boolean - **True** if the specified instance of the [TaskLink](../../com.aspose.tasks/tasklink) class has the same predecessor and successor tasks as this instance; otherwise, **false**.
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
boolean - **True** if the specified object is a TaskLink that has the same predecessor and successor as this instance; otherwise, **false**.
### getCrossProjectName() {#getCrossProjectName--}
```
public final String getCrossProjectName()
```


Gets the external predecessor project.

**Returns:**
java.lang.String - the external predecessor project.
### setCrossProjectName(String value) {#setCrossProjectName-java.lang.String-}
```
public final void setCrossProjectName(String value)
```


Sets the external predecessor project.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the external predecessor project. |

### getLagFormat() {#getLagFormat--}
```
public final int getLagFormat()
```


Gets the format for expressing the lag format.

**Returns:**
int - the format for expressing the lag format.
### setLagFormat(int value) {#setLagFormat-int-}
```
public final void setLagFormat(int value)
```


Sets the format for expressing the lag format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the format for expressing the lag format. |

### getLinkLag() {#getLinkLag--}
```
public final int getLinkLag()
```


Gets the amount of lag in tenths of a minute or percentage.

**Returns:**
int - the amount of lag in tenths of a minute or percentage.
### setLinkLag(int value) {#setLinkLag-int-}
```
public final void setLinkLag(int value)
```


Sets the amount of lag in tenths of a minute or percentage.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the amount of lag in tenths of a minute or percentage. |

### getLinkType() {#getLinkType--}
```
public final int getLinkType()
```


Gets the type of a link.

**Returns:**
int - the type of a link.
### setLinkType(int value) {#setLinkType-int-}
```
public final void setLinkType(int value)
```


Sets the type of a link.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the type of a link. |

### getPredTask() {#getPredTask--}
```
public final Task getPredTask()
```


Gets the predecessor task.

**Returns:**
[Task](../../com.aspose.tasks/task) - the predecessor task.
### setPredTask(Task value) {#setPredTask-com.aspose.tasks.Task-}
```
public final void setPredTask(Task value)
```


Sets the predecessor task.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | the predecessor task. |

### getSuccTask() {#getSuccTask--}
```
public final Task getSuccTask()
```


Gets the successor task.

**Returns:**
[Task](../../com.aspose.tasks/task) - the successor task.
### setSuccTask(Task value) {#setSuccTask-com.aspose.tasks.Task-}
```
public final void setSuccTask(Task value)
```


Sets the successor task.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | the successor task. |

### hashCode() {#hashCode--}
```
public int hashCode()
```


Returns a hash code value for the instance of the [TaskLink](../../com.aspose.tasks/tasklink) class.

**Returns:**
int - returns a hash code value for this object.
### isCrossProject() {#isCrossProject--}
```
public final boolean isCrossProject()
```


Gets a value indicating whether a predecessor is part of another project.

**Returns:**
boolean - a value indicating whether a predecessor is part of another project.
### setCrossProject(boolean value) {#setCrossProject-boolean-}
```
public final void setCrossProject(boolean value)
```


Sets a value indicating whether a predecessor is part of another project.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether a predecessor is part of another project. |

### toString() {#toString--}
```
public String toString()
```


Returns string representation of a TaskLink. The exact details of the representation are unspecified and subject to change.

**Returns:**
java.lang.String - string which represents TaskLink object.
