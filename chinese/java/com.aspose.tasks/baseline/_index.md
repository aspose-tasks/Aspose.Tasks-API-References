---
title: "基线"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示资源的基线值。"
type: docs
weight: 26
url: /zh/java/com.aspose.tasks/baseline/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable, com.aspose.ms.System.IEquatable
```
public class Baseline implements Comparable<Baseline>, System.IEquatable<Baseline>
```

表示资源的基线值。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [Baseline()](#Baseline--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [compareTo(Baseline other)](#compareTo-com.aspose.tasks.Baseline-) | IComparable 接口实现。 |
| [equals(Baseline other)](#equals-com.aspose.tasks.Baseline-) | 返回一个值，指示此实例是否等于指定的对象。 |
| [equals(Object obj)](#equals-java.lang.Object-) | 返回一个值，指示此实例是否等于指定的对象。 |
| [getBaselineNumber()](#getBaselineNumber--) | 获取基线数据记录的唯一编号。 |
| [getBcwp()](#getBcwp--) | 获取资源在项目截至目前执行的工作的预算成本。 |
| [getBcws()](#getBcws--) | 获取为资源计划的工作的预算成本。 |
| [getCost()](#getCost--) | 获取在保存基线时资源的预计成本。 |
| [getWork()](#getWork--) | 获取在保存基线时分配给资源的工作量。 |
| [hashCode()](#hashCode--) | 返回基线的哈希码值。 |
| [op_Equality(Baseline a, Baseline b)](#op-Equality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | 返回一个值，指示此实例是否等于指定的对象。 |
| [op_GreaterThan(Baseline a, Baseline b)](#op-GreaterThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | 返回一个值，指示此实例是否大于指定的对象。 |
| [op_GreaterThanOrEqual(Baseline a, Baseline b)](#op-GreaterThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | 返回一个值，指示此实例是否大于或等于指定的对象。 |
| [op_Inequality(Baseline a, Baseline b)](#op-Inequality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | 返回一个值，指示此实例是否不等于指定的对象。 |
| [op_LessThan(Baseline a, Baseline b)](#op-LessThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | 返回一个值，指示此实例是否小于指定的对象。 |
| [op_LessThanOrEqual(Baseline a, Baseline b)](#op-LessThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | 返回一个值，指示此实例是否小于或等于指定的对象。 |
| [setBaselineNumber(int value)](#setBaselineNumber-int-) | 设置基线数据记录的唯一编号。 |
| [setBcwp(double value)](#setBcwp-double-) | 设置资源在项目截至目前执行的工作的预算成本。 |
| [setBcws(double value)](#setBcws-double-) | 设置为资源计划的工作的预算成本。 |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | 设置在保存基线时资源的预计成本。 |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | 在保存基线时设置分配给资源的工作。 |
### Baseline() {#Baseline--}
```
public Baseline()
```


### compareTo(Baseline other) {#compareTo-com.aspose.tasks.Baseline-}
```
public final int compareTo(Baseline other)
```


IComparable 接口实现。将此实例与指定的 Baseline 对象进行比较。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| other | [Baseline](../../com.aspose.tasks/baseline) | 指定的 Baseline 对象，用于与此实例比较。 |

**Returns:**
int - 如果此实例小于指定对象则返回 -1，若大于指定对象则返回 1；否则返回 0
### equals(Baseline other) {#equals-com.aspose.tasks.Baseline-}
```
public final boolean equals(Baseline other)
```


返回一个值，指示此实例是否等于指定的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| other | [Baseline](../../com.aspose.tasks/baseline) | 指定的对象，用于与此实例比较。 |

**Returns:**
boolean - 如果此实例等于指定对象则返回 true；否则返回 false。
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
### getBaselineNumber() {#getBaselineNumber--}
```
public final int getBaselineNumber()
```


获取基线数据记录的唯一编号。

**Returns:**
int - 基线数据记录的唯一编号。
### getBcwp() {#getBcwp--}
```
public final double getBcwp()
```


获取资源在项目截至目前执行的工作的预算成本。

**Returns:**
double - 资源在项目中截至目前已完成工作的预算成本。
### getBcws() {#getBcws--}
```
public final double getBcws()
```


获取为资源计划的工作的预算成本。

**Returns:**
double - 为资源计划的工作的预算成本。
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


获取在保存基线时资源的预计成本。

**Returns:**
java.math.BigDecimal - 在保存基线时资源的预计成本。
### getWork() {#getWork--}
```
public final Duration getWork()
```


获取在保存基线时分配给资源的工作量。

值：保存基线时分配给资源的工作量。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the work assigned to a resource when the baseline is saved.
### hashCode() {#hashCode--}
```
public int hashCode()
```


返回基线的哈希码值。

**Returns:**
int - 返回此对象的哈希码值。
### op_Equality(Baseline a, Baseline b) {#op-Equality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_Equality(Baseline a, Baseline b)
```


返回一个值，指示此实例是否等于指定的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | 第一个基线。 |
| b | [Baseline](../../com.aspose.tasks/baseline) | 第二个基线。 |

**Returns:**
boolean - 一个值，指示此实例是否等于指定的对象
### op_GreaterThan(Baseline a, Baseline b) {#op-GreaterThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_GreaterThan(Baseline a, Baseline b)
```


返回一个值，指示此实例是否大于指定的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | 第一个基线。 |
| b | [Baseline](../../com.aspose.tasks/baseline) | 第二个基线。 |

**Returns:**
boolean - 一个值，指示此实例是否大于指定的对象
### op_GreaterThanOrEqual(Baseline a, Baseline b) {#op-GreaterThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_GreaterThanOrEqual(Baseline a, Baseline b)
```


返回一个值，指示此实例是否大于或等于指定的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | 第一个基线。 |
| b | [Baseline](../../com.aspose.tasks/baseline) | 第二个基线。 |

**Returns:**
boolean - 一个值，指示此实例是否大于或等于指定的对象
### op_Inequality(Baseline a, Baseline b) {#op-Inequality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_Inequality(Baseline a, Baseline b)
```


返回一个值，指示此实例是否不等于指定的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | 第一个基线。 |
| b | [Baseline](../../com.aspose.tasks/baseline) | 第二个基线。 |

**Returns:**
boolean - 一个值，指示此实例是否不等于指定的对象
### op_LessThan(Baseline a, Baseline b) {#op-LessThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_LessThan(Baseline a, Baseline b)
```


返回一个值，指示此实例是否小于指定的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | 第一个基线。 |
| b | [Baseline](../../com.aspose.tasks/baseline) | 第二个基线。 |

**Returns:**
boolean - 一个值，指示此实例是否小于指定的对象
### op_LessThanOrEqual(Baseline a, Baseline b) {#op-LessThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_LessThanOrEqual(Baseline a, Baseline b)
```


返回一个值，指示此实例是否小于或等于指定的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | 第一个基线。 |
| b | [Baseline](../../com.aspose.tasks/baseline) | 第二个基线。 |

**Returns:**
boolean - 一个值，指示此实例是否小于或等于指定的对象
### setBaselineNumber(int value) {#setBaselineNumber-int-}
```
public final void setBaselineNumber(int value)
```


设置基线数据记录的唯一编号。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 基线数据记录的唯一编号。 |

### setBcwp(double value) {#setBcwp-double-}
```
public final void setBcwp(double value)
```


设置资源在项目截至目前执行的工作的预算成本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | 资源在项目中截至目前已完成工作的预算成本。 |

### setBcws(double value) {#setBcws-double-}
```
public final void setBcws(double value)
```


设置为资源计划的工作的预算成本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | 为资源计划的工作的预算成本。 |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


设置在保存基线时资源的预计成本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.math.BigDecimal | 在保存基线时资源的预计成本。 |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


在保存基线时设置分配给资源的工作。

值：保存基线时分配给资源的工作量。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | 在保存基线时分配给资源的工作。 |

