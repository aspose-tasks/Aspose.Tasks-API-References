---
title: "Rsc.OvertimeCost"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。资源在所有分配任务上的总加班成本"
type: docs
weight: 500
url: /zh/net/aspose.tasks/rsc/overtimecost/
---
## Rsc.OvertimeCost field

资源在所有分配任务上的加班总成本。

```csharp
public static readonly Key<decimal, RscKey> OvertimeCost;
```

## 示例

展示如何读取资源加班值。

```csharp
var project = new Project(DataDir + "ResourceOvertime.mpp");

// 显示所有资源的加班相关参数
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) == null)
    {
        continue;
    }

    Console.WriteLine(res.Get(Rsc.OvertimeCost));
    Console.WriteLine(res.Get(Rsc.OvertimeWork).ToString());
    Console.WriteLine(res.Get(Rsc.OvertimeRateFormat).ToString());
}
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


