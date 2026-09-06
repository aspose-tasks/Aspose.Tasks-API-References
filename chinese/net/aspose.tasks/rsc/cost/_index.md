---
title: "Rsc.Cost"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。基于已发生的成本（由分配到任务的资源完成的工作产生的成本）以及对剩余工作计划的成本，对资源的总计划或预计成本"
type: docs
weight: 220
url: /zh/net/aspose.tasks/rsc/cost/
---
## Rsc.Cost field

资源的总计划或预测成本，基于已分配给任务的资源完成的工作已产生的成本，以及剩余工作计划的成本。

```csharp
public static readonly Key<decimal, RscKey> Cost;
```

## 示例

展示如何读取资源成本。

```csharp
var project = new Project(DataDir + "ResourceCosts.mpp");

// 显示所有资源成本
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) == null)
    {
        continue;
    }

    Console.WriteLine(res.Get(Rsc.Cost));
    Console.WriteLine(res.Get(Rsc.ACWP));
    Console.WriteLine(res.Get(Rsc.BCWS));
    Console.WriteLine(res.Get(Rsc.BCWP));

    // CV = BCWP - ACWP
    Console.WriteLine(res.Get(Rsc.CV));

    // SV = BCWP - BCWS
    Console.WriteLine(res.Get(Rsc.SV));
}
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


