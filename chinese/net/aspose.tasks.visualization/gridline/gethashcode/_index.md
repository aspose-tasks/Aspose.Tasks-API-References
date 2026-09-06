---
title: "Gridline.GetHashCode"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Gridline 方法。返回 Gridline 类实例的哈希码值"
type: docs
weight: 60
url: /zh/net/aspose.tasks.visualization/gridline/gethashcode/
---
## Gridline.GetHashCode method

返回 [`Gridline`](../) 类实例的哈希码值。

```csharp
public override int GetHashCode()
```

### 返回值

返回此对象的哈希码值。

## 示例

展示如何获取网格线的哈希码。

```csharp
var gridline1 = new Gridline();
var gridline2 = new Gridline();

// 网格线的哈希码基于内部 GUID 字段。
Console.WriteLine("Gridline 1 Hash Code: {0}", gridline1.GetHashCode());
Console.WriteLine("Gridline 2 Hash Code: {0}", gridline2.GetHashCode());
```

### 另见

* class [Gridline](../)
* namespace [Aspose.Tasks.Visualization](../../gridline/)
* assembly [Aspose.Tasks](../../../)


