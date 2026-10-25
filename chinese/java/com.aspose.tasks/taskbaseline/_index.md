---
title: "TaskBaseline"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示任务的基线。"
type: docs
weight: 291
url: /zh/java/com.aspose.tasks/taskbaseline/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.Baseline](../../com.aspose.tasks/baseline)

**All Implemented Interfaces:**
java.lang.Comparable
```
public class TaskBaseline extends Baseline implements Comparable<Baseline>
```

表示任务的基线。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [TaskBaseline(Task task)](#TaskBaseline-com.aspose.tasks.Task-) | 初始化一个新的 [TaskBaseline](../../com.aspose.tasks/taskbaseline) 类实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [compareTo(TaskBaseline other)](#compareTo-com.aspose.tasks.TaskBaseline-) | IComparable 接口实现。 |
| [equals(TaskBaseline other)](#equals-com.aspose.tasks.TaskBaseline-) | 返回一个值，指示此实例是否等于指定的 TaskBaseline 对象。 |
| [equals(Object obj)](#equals-java.lang.Object-) | 返回一个值，指示此实例是否等于指定的对象。 |
| [getDuration()](#getDuration--) | 获取基线保存时任务的计划持续时间。 |
| [getEstimatedDuration()](#getEstimatedDuration--) | 获取一个值，指示任务的基线持续时间是否为估计值。 |
| [getFinish()](#getFinish--) | 获取基线保存时任务的计划完成日期。 |
| [getFixedCost()](#getFixedCost--) | 获取基线保存时任务的固定成本。 |
| [getInterim()](#getInterim--) | 获取一个值，指示这是否为临时基线。 |
| [getStart()](#getStart--) | 获取基线保存时任务的计划开始日期。 |
| [getTimephasedData()](#getTimephasedData--) | 获取此对象的 TimephasedDataCollection 实例。 |
| [hashCode()](#hashCode--) | 返回 [TaskBaseline](../../com.aspose.tasks/taskbaseline) 类实例的哈希码值。 |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | 设置基线保存时任务的计划持续时间。 |
| [setEstimatedDuration(boolean value)](#setEstimatedDuration-boolean-) | 设置一个值，指示任务的基线持续时间是否为估计值。 |
| [setFinish(Date value)](#setFinish-java.util.Date-) | 设置基线保存时任务的计划完成日期。 |
| [setFixedCost(double value)](#setFixedCost-double-) | 设置基线保存时任务的固定成本。 |
| [setInterim(boolean value)](#setInterim-boolean-) | 设置一个值，指示这是否为临时基线。 |
| [setStart(Date value)](#setStart-java.util.Date-) | 设置基线保存时任务的计划开始日期。 |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | 设置此对象的 TimephasedDataCollection 实例。 |
### TaskBaseline(Task task) {#TaskBaseline-com.aspose.tasks.Task-}
```
public TaskBaseline(Task task)
```


初始化一个新的 [TaskBaseline](../../com.aspose.tasks/taskbaseline) 类实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | 基线的父任务。 |

### compareTo(TaskBaseline other) {#compareTo-com.aspose.tasks.TaskBaseline-}
```
public final int compareTo(TaskBaseline other)
```


IComparable 接口实现。将此实例与指定的 Baseline 对象进行比较。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| other | [TaskBaseline](../../com.aspose.tasks/taskbaseline) | 指定的 Baseline 对象，用于与此实例比较。 |

**Returns:**
int - 如果此实例小于指定对象则返回 -1，若大于指定对象则返回 1；否则返回 0
### equals(TaskBaseline other) {#equals-com.aspose.tasks.TaskBaseline-}
```
public final boolean equals(TaskBaseline other)
```


返回一个值，指示此实例是否等于指定的 TaskBaseline 对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| other | [TaskBaseline](../../com.aspose.tasks/taskbaseline) | 要与此实例比较的指定 AssignmentBaseline 对象。 |

**Returns:**
boolean - 如果此实例等于指定的 TaskBaseline 对象则返回 true；否则返回 false。
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
boolean - **True** 如果指定的对象是具有相同 UID 值的 TaskBaseline 实例；否则，**false**。
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


获取基线保存时任务的计划持续时间。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the scheduled duration of the task when the baseline was saved.
### getEstimatedDuration() {#getEstimatedDuration--}
```
public final boolean getEstimatedDuration()
```


获取一个值，指示任务的基线持续时间是否为估计值。

**Returns:**
boolean - 指示任务的基线持续时间是否为估计值的标志。
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


获取基线保存时任务的计划完成日期。

**Returns:**
java.util.Date - 基线保存时任务的计划完成日期。
### getFixedCost() {#getFixedCost--}
```
public final double getFixedCost()
```


获取基线保存时任务的固定成本。

**Returns:**
double - 基线保存时任务的固定成本。
### getInterim() {#getInterim--}
```
public final boolean getInterim()
```


获取一个值，指示这是否为临时基线。

**Returns:**
boolean - 表示此是否为临时基线的值。
### getStart() {#getStart--}
```
public final Date getStart()
```


获取基线保存时任务的计划开始日期。

**Returns:**
java.util.Date - 基线保存时任务的计划开始日期。
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


获取此对象的 TimephasedDataCollection 实例。与任务基线关联的时间分段数据。

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - a TimephasedDataCollection instance for this object.
### hashCode() {#hashCode--}
```
public int hashCode()
```


返回 [TaskBaseline](../../com.aspose.tasks/taskbaseline) 类实例的哈希码值。

**Returns:**
int - 返回此对象的哈希码值。
### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


设置基线保存时任务的计划持续时间。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | 基线保存时任务的计划持续时间。 |

### setEstimatedDuration(boolean value) {#setEstimatedDuration-boolean-}
```
public final void setEstimatedDuration(boolean value)
```


设置一个值，指示任务的基线持续时间是否为估计值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 表示任务基线持续时间是否为估计值的标识。 |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


设置基线保存时任务的计划完成日期。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | 基线保存时任务的计划完成日期。 |

### setFixedCost(double value) {#setFixedCost-double-}
```
public final void setFixedCost(double value)
```


设置基线保存时任务的固定成本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | 基线保存时任务的固定成本。 |

### setInterim(boolean value) {#setInterim-boolean-}
```
public final void setInterim(boolean value)
```


设置一个值，指示这是否为临时基线。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 表示此是否为临时基线的值。 |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


设置基线保存时任务的计划开始日期。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | 基线保存时任务的计划开始日期。 |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


设置此对象的 TimephasedDataCollection 实例。与任务基线关联的时间分段数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | 此对象的 TimephasedDataCollection 实例。 |

