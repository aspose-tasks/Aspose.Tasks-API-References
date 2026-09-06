---
title: "Rsc.CV"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。项目状态日期截至的挣值成本差异。CV 是任务的 BCWP（已完成工作预算成本）与 ACWP（实际完成工作成本）之间的差额"
type: docs
weight: 270
url: /zh/net/aspose.tasks/rsc/cv/
---
## Rsc.CV field

截至项目状态日期的挣值成本差异。CV 是任务的已完成工作预算成本（BCWP）与实际完成工作成本（ACWP）之间的差额。

```csharp
public static readonly Key<double, RscKey> CV;
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


