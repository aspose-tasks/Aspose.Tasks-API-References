---
title: "Rsc.OvertimeWork"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。资源在任务上计划执行的加班时间量，并按相关资源的加班费率计费"
type: docs
weight: 530
url: /zh/net/aspose.tasks/rsc/overtimework/
---
## Rsc.OvertimeWork field

计划资源在任务上执行的加班量，并按相关资源的加班率计费。

```csharp
public static readonly Key<Duration, RscKey> OvertimeWork;
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
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


