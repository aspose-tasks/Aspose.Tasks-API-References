---
title: "Rsc.RemainingOvertimeCost"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。资源剩余的计划加班费用"
type: docs
weight: 590
url: /zh/net/aspose.tasks/rsc/remainingovertimecost/
---
## Rsc.RemainingOvertimeCost field

资源的剩余计划加班费用。

```csharp
public static readonly Key<decimal, RscKey> RemainingOvertimeCost;
```

## 示例

展示如何读取/写入 Rsc.RemainingOvertimeCost 属性。

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingOvertimeCost, 3);

Console.WriteLine("Remaining Overtime Cost: " + resource.Get(Rsc.RemainingOvertimeCost));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


