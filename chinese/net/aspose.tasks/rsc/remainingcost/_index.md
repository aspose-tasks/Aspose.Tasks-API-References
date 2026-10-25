---
title: "Rsc.RemainingCost"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。完成剩余计划工作时将产生的剩余计划费用"
type: docs
weight: 580
url: /zh/net/aspose.tasks/rsc/remainingcost/
---
## Rsc.RemainingCost field

完成剩余计划工作将产生的剩余计划费用。

```csharp
public static readonly Key<decimal, RscKey> RemainingCost;
```

## 示例

展示如何读取/写入 Rsc.RemainingCost 属性。

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingCost, 2);

Console.WriteLine("Remaining Cost: " + resource.Get(Rsc.RemainingCost));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


