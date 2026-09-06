---
title: "Prj.SpreadActualCost"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。确定实际成本是否分摊到状态日期"
type: docs
weight: 660
url: /zh/net/aspose.tasks/prj/spreadactualcost/
---
## Prj.SpreadActualCost field

确定实际成本是否分摊到状态日期。

```csharp
public static readonly Key<NullableBool, PrjKey> SpreadActualCost;
```

## 示例

展示如何读取/写入 Prj.SpreadActualCost 属性。

```csharp
var project = new Project();

project.Set(Prj.SpreadActualCost, true);

Console.WriteLine("Spread Actual Cost: " + project.Get(Prj.SpreadActualCost));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


