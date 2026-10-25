---
title: "Rsc.ACWP"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。资源在项目中截至目前执行的工作实际成本"
type: docs
weight: 90
url: /zh/net/aspose.tasks/rsc/acwp/
---
## Rsc.ACWP field

截至目前资源为项目执行的工作的实际成本。

```csharp
public static readonly Key<double, RscKey> ACWP;
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


