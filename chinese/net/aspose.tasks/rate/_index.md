---
title: "类 Rate"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Rate 类。表示一个时间段的定义以及该期间资源适用的费率。"
type: docs
weight: 1610
url: /zh/net/aspose.tasks/rate/
---
## Rate class

表示在该期间适用于资源的时间段和费率的定义。

```csharp
public class Rate
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [CostPerUse](../../aspose.tasks/rate/costperuse/) { get; set; } | 获取或设置资源每次使用的成本。如果资源存在费率表，则此值从当前日期获取。 |
| [OvertimeRate](../../aspose.tasks/rate/overtimerate/) { get; set; } | 获取或设置资源每小时的加班费率。 |
| [OvertimeRateFormat](../../aspose.tasks/rate/overtimerateformat/) { get; set; } | 获取或设置 Microsoft Project 用于显示加班费率的单位。 |
| [RatesFrom](../../aspose.tasks/rate/ratesfrom/) { get; set; } | 获取或设置费率生效的日期。 |
| [RatesTo](../../aspose.tasks/rate/ratesto/) { get; set; } | 获取或设置费率有效的最后日期。 |
| [RateTable](../../aspose.tasks/rate/ratetable/) { get; set; } | 获取或设置资源费率表的唯一标识符。 |
| [StandardRate](../../aspose.tasks/rate/standardrate/) { get; set; } | 获取或设置资源每小时的标准费率。 |
| [StandardRateFormat](../../aspose.tasks/rate/standardrateformat/) { get; set; } | 获取或设置 Microsoft Project 用于显示标准费率的单位。 |

## 示例

展示如何使用资源费率。

```csharp
var project = new Project(DataDir + "Project1.mpp");

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);
resource.Set(Rsc.Work, project.GetDuration(2d, TimeUnitType.Hour));
resource.Set(Rsc.StandardRate, 20m);

var rate1 = resource.Rates.Add(new DateTime(2019, 1, 1, 8, 0, 0));
rate1.RateTable = RateType.A;
rate1.RatesFrom = new DateTime(2019, 1, 1, 8, 0, 0);
rate1.RatesTo = new DateTime(2019, 11, 11, 17, 0, 0);
rate1.StandardRate = 5m;
rate1.StandardRateFormat = RateFormatType.Hour;
rate1.OvertimeRate = 10m;
rate1.OvertimeRateFormat = RateFormatType.Hour;

var rate2 = resource.Rates.Add(new DateTime(2019, 11, 12, 8, 0, 0));
rate2.RatesTo = new DateTime(2019, 12, 31, 17, 0, 0);
rate2.StandardRate = 10m;
rate2.StandardRateFormat = RateFormatType.Hour;
rate2.CostPerUse = 2m;

// 处理项目...
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


