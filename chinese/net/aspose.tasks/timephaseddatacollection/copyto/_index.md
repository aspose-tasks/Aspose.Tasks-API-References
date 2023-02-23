---
title: TimephasedDataCollection.CopyTo
second_title: Aspose.Tasks for .NET API 参考
description: TimephasedDataCollection 方法. 复制元素TimephasedDataCollection到一个Array 从特定的开始Array索引.
type: docs
weight: 90
url: /zh/net/aspose.tasks/timephaseddatacollection/copyto/
---
## TimephasedDataCollection.CopyTo method

复制元素[`TimephasedDataCollection`](../)到一个Array, 从特定的开始Array索引.

```csharp
public void CopyTo(TimephasedData[] array, int arrayIndex)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| array | TimephasedData[] | 一维的Array这是从中复制的元素的目的地[`TimephasedDataCollection`](../). 的Array必须具有从零开始的索引。 |
| arrayIndex | Int32 | 从零开始的指数*array*复制开始的位置。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentNullException | *array*一片空白。 |
| ArgumentOutOfRangeException | *arrayIndex*小于 0。 |
| ArgumentException | 源中的元素数[`TimephasedDataCollection`](../) 大于可用空间*arrayIndex*到目的地的尽头*array*. |

### 也可以看看

* class [TimephasedData](../../timephaseddata/)
* class [TimephasedDataCollection](../)
* 命名空间 [Aspose.Tasks](../../timephaseddatacollection/)
* 部件 [Aspose.Tasks](../../../)


