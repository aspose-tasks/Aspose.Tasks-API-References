---
title: "AssignmentBaseline"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示资源分配的基线。"
type: docs
weight: 17
url: /zh/java/com.aspose.tasks/assignmentbaseline/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.Baseline](../../com.aspose.tasks/baseline)
```
public class AssignmentBaseline extends Baseline
```

表示资源分配的基线。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [AssignmentBaseline()](#AssignmentBaseline--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [compareTo(AssignmentBaseline other)](#compareTo-com.aspose.tasks.AssignmentBaseline-) | IComparable 接口实现。 |
| [equals(AssignmentBaseline other)](#equals-com.aspose.tasks.AssignmentBaseline-) | 返回一个值，指示此实例是否等于指定的 AssignmentBaseline 对象。 |
| [equals(Object obj)](#equals-java.lang.Object-) | 返回一个值，指示此实例是否等于指定的对象。 |
| [getFinish()](#getFinish--) | 获取基线保存时资源分配的计划完成日期。 |
| [getStart()](#getStart--) | 获取基线保存时资源分配的计划开始日期。 |
| [getTimephasedData()](#getTimephasedData--) | 获取此对象的 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 实例。 |
| [hashCode()](#hashCode--) | 返回此 AssignmentBaseline 的哈希码值。 |
| [setFinish(Date value)](#setFinish-java.util.Date-) | 设置基线保存时资源分配的计划完成日期。 |
| [setStart(Date value)](#setStart-java.util.Date-) | 设置基线保存时资源分配的计划开始日期。 |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | 为此对象设置 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 实例。 |
### AssignmentBaseline() {#AssignmentBaseline--}
```
public AssignmentBaseline()
```


### compareTo(AssignmentBaseline other) {#compareTo-com.aspose.tasks.AssignmentBaseline-}
```
public final int compareTo(AssignmentBaseline other)
```


IComparable 接口实现。将此实例与指定的 Baseline 对象进行比较。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| other | [AssignmentBaseline](../../com.aspose.tasks/assignmentbaseline) | 指定的 Baseline 对象，用于与此实例比较。 |

**Returns:**
int - 如果此实例小于指定对象则返回 -1，若大于指定对象则返回 1；否则返回 0
### equals(AssignmentBaseline other) {#equals-com.aspose.tasks.AssignmentBaseline-}
```
public final boolean equals(AssignmentBaseline other)
```


返回一个值，指示此实例是否等于指定的 AssignmentBaseline 对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| other | [AssignmentBaseline](../../com.aspose.tasks/assignmentbaseline) | 要与此实例比较的指定 AssignmentBaseline 对象。 |

**Returns:**
boolean - 如果此实例等于指定的 AssignmentBaseline 对象则返回 true；否则返回 false。
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


返回一个值，指示此实例是否等于指定的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | java.lang.Object | 指定的对象，用于与此实例比较。 |

**Returns:**
boolean - 如果此实例等于指定对象则返回 true；否则返回 false。
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


获取基线保存时资源分配的计划完成日期。

值：保存此基线时资源分配的完成日期。

**Returns:**
java.util.Date - 保存基线时资源分配的计划完成日期。
### getStart() {#getStart--}
```
public final Date getStart()
```


获取基线保存时资源分配的计划开始日期。

值：保存此基线时资源分配的开始日期。

**Returns:**
java.util.Date - 保存基线时资源分配的计划开始日期。
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


获取此对象的 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 实例。与资源分配基线关联的时间分段数据。

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) instance for this object. Value: The collection of Time phased data associated with this baseline.
### hashCode() {#hashCode--}
```
public int hashCode()
```


返回此 AssignmentBaseline 的哈希码值。

**Returns:**
int - 返回此对象的哈希码值。
### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


设置基线保存时资源分配的计划完成日期。

值：保存此基线时资源分配的完成日期。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | 保存基线时资源分配的计划完成日期。 |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


设置基线保存时资源分配的计划开始日期。

值：保存此基线时资源分配的开始日期。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | 保存基线时资源分配的计划开始日期。 |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


为此对象设置 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 实例。与资源分配基线关联的时间分段数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | 此对象的 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 实例。 |

