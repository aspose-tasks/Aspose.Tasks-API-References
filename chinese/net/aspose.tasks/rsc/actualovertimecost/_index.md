---
title: "Rsc.ActualOvertimeCost"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。已分配资源在任务上已完成的加班工作产生的费用"
type: docs
weight: 40
url: /zh/net/aspose.tasks/rsc/actualovertimecost/
---
## Rsc.ActualOvertimeCost field

指派资源在任务上已完成的加班工作产生的费用。

```csharp
public static readonly Key<decimal, RscKey> ActualOvertimeCost;
```

## 示例

展示如何读取/写入 Rsc.ActualOvertimeCost 属性。

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeCost, 10m);

Console.WriteLine("Actual Overtime Cost: " + resource.Get(Rsc.ActualOvertimeCost));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


