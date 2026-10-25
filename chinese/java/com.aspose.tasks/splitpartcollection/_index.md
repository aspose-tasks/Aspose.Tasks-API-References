---
title: "SplitPartCollection"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示任务各部分的集合。"
type: docs
weight: 279
url: /zh/java/com.aspose.tasks/splitpartcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class SplitPartCollection extends AbstractList<SplitPart>
```

表示任务各部分的集合。
## 方法

| 方法 | 描述 |
| --- | --- |
| [get(int index)](#get-int-) | 检索任务在给定索引处的拆分部分。 |
| [set(int index, SplitPart value)](#set-int-com.aspose.tasks.SplitPart-) | 设置任务在给定索引处的拆分部分。 |
| [size()](#size--) | 获取集合中部分的数量。 |
| [toArray()](#toArray--) | 将集合中的所有部分复制到新数组。 |
### get(int index) {#get-int-}
```
public final SplitPart get(int index)
```


检索任务在给定索引处的拆分部分。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 索引 | int | 部分索引。 |

--------------------

索引从零开始。如果索引超出数组边界，则返回 null。 |

**Returns:**
[SplitPart](../../com.aspose.tasks/splitpart) - a split part.
### set(int index, SplitPart value) {#set-int-com.aspose.tasks.SplitPart-}
```
public final SplitPart set(int index, SplitPart value)
```


设置任务在给定索引处的拆分部分。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 索引 | int | 部分索引。 |

--------------------

索引从零开始。如果索引超出数组边界，则返回 null。 |
| value | [SplitPart](../../com.aspose.tasks/splitpart) | 要设置的拆分部分。 |

**Returns:**
[SplitPart](../../com.aspose.tasks/splitpart) - a split part.
### size() {#size--}
```
public final int size()
```


获取集合中部分的数量。

**Returns:**
int - 集合中部分的数量。
### toArray() {#toArray--}
```
public final SplitPart[] toArray()
```


将集合中的所有部分复制到新数组。

**Returns:**
com.aspose.tasks.SplitPart[] - 一个 [SplitPart](../../com.aspose.tasks/splitpart) 对象数组。
