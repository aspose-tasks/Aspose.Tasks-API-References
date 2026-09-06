---
title: "Gridline.Equals"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Gridline 方法。返回一个标志，指示此实例是否等于指定的对象"
type: docs
weight: 50
url: /zh/net/aspose.tasks.visualization/gridline/equals/
---
## Gridline.Equals method

返回一个标志，指示此实例是否等于指定的对象。

```csharp
public override bool Equals(object obj)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | 对象 | 用于与此实例比较的指定对象。 |

### 返回值

一个标志，指示此实例是否等于指定的对象。

## 示例

展示如何检查网格线的相等性。

```csharp
var gridline1 = new Gridline();
var gridline2 = new Gridline();

// 网格线的相等性是针对网格线类型进行检查的。
Console.WriteLine("Gridline 1 Type: " + gridline1.GridlineType);
Console.WriteLine("Gridline 2 Type: " + gridline2.GridlineType);
Console.WriteLine("Are gridlines equal: " + gridline1.Equals(gridline2));

// 更改类型
gridline1.GridlineType = GridlineType.BarRows;
Console.WriteLine("Gridline 1 Type: " + gridline1.GridlineType);
Console.WriteLine("Are gridlines equal: " + gridline1.Equals(gridline2));
```

### 另见

* class [Gridline](../)
* namespace [Aspose.Tasks.Visualization](../../gridline/)
* assembly [Aspose.Tasks](../../../)


