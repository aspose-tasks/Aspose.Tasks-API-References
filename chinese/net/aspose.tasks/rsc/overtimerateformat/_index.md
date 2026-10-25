---
title: "Rsc.OvertimeRateFormat"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。Microsoft Project 用于显示加班费率的单位"
type: docs
weight: 520
url: /zh/net/aspose.tasks/rsc/overtimerateformat/
---
## Rsc.OvertimeRateFormat field

Microsoft Project 用于显示加班率的单位。

```csharp
public static readonly Key<RateFormatType, RscKey> OvertimeRateFormat;
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
* enum [RateFormatType](../../rateformattype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


