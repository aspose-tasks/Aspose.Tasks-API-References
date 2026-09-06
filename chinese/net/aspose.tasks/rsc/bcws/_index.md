---
title: "Rsc.BCWS"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。为资源安排的工作的预算成本"
type: docs
weight: 150
url: /zh/net/aspose.tasks/rsc/bcws/
---
## Rsc.BCWS field

为资源计划的工作的预算成本。

```csharp
public static readonly Key<double, RscKey> BCWS;
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


