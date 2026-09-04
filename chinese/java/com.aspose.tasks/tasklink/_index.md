---
title: "TaskLink"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示前置链接。"
type: docs
weight: 295
url: /zh/java/com.aspose.tasks/tasklink/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable
```
public final class TaskLink implements System.IEquatable<TaskLink>
```

表示前置链接。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(TaskLink other)](#equals-com.aspose.tasks.TaskLink-) | 返回一个值，指示此实例是否等于指定的对象。 |
| [equals(Object obj)](#equals-java.lang.Object-) | 返回一个值，指示此实例是否等于指定的对象。 |
| [getCrossProjectName()](#getCrossProjectName--) | 获取外部前置项目。 |
| [getLagFormat()](#getLagFormat--) | 获取用于表示延迟格式的格式。 |
| [getLinkLag()](#getLinkLag--) | 获取以十分之一分钟或百分比表示的延迟。 |
| [getLinkLagTimeSpan()](#getLinkLagTimeSpan--) | 获取延迟持续时间，取决于 LagFormat。 |
| [getLinkType()](#getLinkType--) | 获取链接的类型。 |
| [getPredTask()](#getPredTask--) | 获取前置任务。 |
| [getSuccTask()](#getSuccTask--) | 获取后置任务。 |
| [hashCode()](#hashCode--) | 返回 [TaskLink](../../com.aspose.tasks/tasklink) 类实例的哈希码值。 |
| [isCrossProject()](#isCrossProject--) | 获取一个值，指示前置任务是否属于另一个项目。 |
| [setCrossProject(boolean value)](#setCrossProject-boolean-) | 设置一个值，指示前置任务是否属于另一个项目。 |
| [setCrossProjectName(String value)](#setCrossProjectName-java.lang.String-) | 设置外部前置项目。 |
| [setLagFormat(byte value)](#setLagFormat-byte-) | 设置用于表达延迟格式的格式。 |
| [setLinkLag(int value)](#setLinkLag-int-) | 设置以十分之一分钟或百分比表示的延迟。 |
| [setLinkLagTimeSpan(double value)](#setLinkLagTimeSpan-double-) | 根据 LagFormat 设置延迟持续时间。 |
| [setLinkType(int value)](#setLinkType-int-) | 设置链接的类型。 |
| [setPredTask(Task value)](#setPredTask-com.aspose.tasks.Task-) | 设置前置任务。 |
| [setSuccTask(Task value)](#setSuccTask-com.aspose.tasks.Task-) | 设置后置任务。 |
| [toString()](#toString--) | 返回 TaskLink 的字符串表示形式。 |
### equals(TaskLink other) {#equals-com.aspose.tasks.TaskLink-}
```
public final boolean equals(TaskLink other)
```


返回一个值，指示此实例是否等于指定的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| other | [TaskLink](../../com.aspose.tasks/tasklink) | 要与此实例比较的指定 [TaskLink](../../com.aspose.tasks/tasklink) 类实例。 |

**Returns:**
boolean - **True** 如果指定的 [TaskLink](../../com.aspose.tasks/tasklink) 类实例与此实例具有相同的前置和后置任务；否则，**false**。
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


返回一个值，指示此实例是否等于指定的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | java.lang.Object | 用于与此实例比较的对象。 |

**Returns:**
boolean - **True** 如果指定的对象是具有与此实例相同前置和后置的 TaskLink；否则，**false**。
### getCrossProjectName() {#getCrossProjectName--}
```
public final String getCrossProjectName()
```


获取外部前置项目。

**Returns:**
java.lang.String - 外部前置项目。
### getLagFormat() {#getLagFormat--}
```
public final byte getLagFormat()
```


获取用于表示延迟格式的格式。

**Returns:**
byte - 用于表达延迟格式的格式。
### getLinkLag() {#getLinkLag--}
```
public final int getLinkLag()
```


获取以十分之一分钟或百分比表示的延迟。

**Returns:**
int - 以十分之一分钟或百分比表示的延迟。
### getLinkLagTimeSpan() {#getLinkLagTimeSpan--}
```
public final double getLinkLagTimeSpan()
```


获取延迟持续时间，取决于 LagFormat。

**Returns:**
double - 延迟持续时间，取决于 LagFormat。
### getLinkType() {#getLinkType--}
```
public final int getLinkType()
```


获取链接的类型。

**Returns:**
int - 链接的类型。
### getPredTask() {#getPredTask--}
```
public final Task getPredTask()
```


获取前置任务。

**Returns:**
[Task](../../com.aspose.tasks/task) - the predecessor task.
### getSuccTask() {#getSuccTask--}
```
public final Task getSuccTask()
```


获取后置任务。

**Returns:**
[Task](../../com.aspose.tasks/task) - the successor task.
### hashCode() {#hashCode--}
```
public int hashCode()
```


返回 [TaskLink](../../com.aspose.tasks/tasklink) 类实例的哈希码值。

**Returns:**
int - 返回此对象的哈希码值。
### isCrossProject() {#isCrossProject--}
```
public final boolean isCrossProject()
```


获取一个值，指示前置任务是否属于另一个项目。

**Returns:**
boolean - 一个值，指示前置任务是否属于另一个项目。
### setCrossProject(boolean value) {#setCrossProject-boolean-}
```
public final void setCrossProject(boolean value)
```


设置一个值，指示前置任务是否属于另一个项目。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 一个值，指示前置任务是否属于另一个项目。 |

### setCrossProjectName(String value) {#setCrossProjectName-java.lang.String-}
```
public final void setCrossProjectName(String value)
```


设置外部前置项目。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 外部前置项目。 |

### setLagFormat(byte value) {#setLagFormat-byte-}
```
public final void setLagFormat(byte value)
```


设置用于表达延迟格式的格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | 字节 | 用于表达延迟格式的格式。 |

### setLinkLag(int value) {#setLinkLag-int-}
```
public final void setLinkLag(int value)
```


设置以十分之一分钟或百分比表示的延迟。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 以十分之一分钟或百分比表示的延迟。 |

### setLinkLagTimeSpan(double value) {#setLinkLagTimeSpan-double-}
```
public final void setLinkLagTimeSpan(double value)
```


根据 LagFormat 设置延迟持续时间。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | 延迟持续时间，取决于 LagFormat。 |

### setLinkType(int value) {#setLinkType-int-}
```
public final void setLinkType(int value)
```


设置链接的类型。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 链接的类型。 |

### setPredTask(Task value) {#setPredTask-com.aspose.tasks.Task-}
```
public final void setPredTask(Task value)
```


设置前置任务。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | 前置任务。 |

### setSuccTask(Task value) {#setSuccTask-com.aspose.tasks.Task-}
```
public final void setSuccTask(Task value)
```


设置后置任务。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | 后续任务。 |

### toString() {#toString--}
```
public String toString()
```


返回 TaskLink 的字符串表示形式。表示的具体细节未指定，可能会更改。

**Returns:**
java.lang.String - 表示 TaskLink 对象的字符串。
