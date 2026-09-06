---
title: "类 AvailabilityPeriod"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.AvailabilityPeriod 类。表示资源可用的期间"
type: docs
weight: 80
url: /zh/net/aspose.tasks/availabilityperiod/
---
## AvailabilityPeriod class

表示资源可用的时间段。

```csharp
public class AvailabilityPeriod
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [AvailabilityPeriod](availabilityperiod/#constructor)() | 初始化 `AvailabilityPeriod` 的新实例。 |
| [AvailabilityPeriod](availabilityperiod/#constructor_1)(DateTime, DateTime, double) | 使用指定的日期范围和可用单位初始化 `AvailabilityPeriod` 的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [AvailableFrom](../../aspose.tasks/availabilityperiod/availablefrom/) { get; set; } | 获取或设置资源在指定期间可用的日期。 |
| [AvailableTo](../../aspose.tasks/availabilityperiod/availableto/) { get; set; } | 获取或设置资源在指定期间可用的最后日期。 |
| [AvailableUnits](../../aspose.tasks/availabilityperiod/availableunits/) { get; set; } | 获取或设置资源在指定期间可用的百分比。 |

## 示例

展示如何为资源创建可用期间。

```csharp
public void WorkWithAvailabilityPeriod()
{
    var project = new Project();
    var resource = project.Resources.Add("Work Resource");

    // 向新资源添加可用期间
    IEnumerable<AvailabilityPeriod> periods = GetPeriods();
    foreach (var period in periods)
    {
        resource.AvailabilityPeriods.Add(period);
    }

    foreach (var period in resource.AvailabilityPeriods)
    {
        Console.WriteLine("Available From: " + period.AvailableFrom);
        Console.WriteLine("Available To: " + period.AvailableTo);
        Console.WriteLine("Available Units: " + period.AvailableUnits);
        Console.WriteLine();
    }
}

private static IEnumerable<AvailabilityPeriod> GetPeriods()
{
    var periods = new List<AvailabilityPeriod>(2);
    var period = new AvailabilityPeriod
    {
        AvailableFrom = new DateTime(2011, 12, 12),
        AvailableTo = new DateTime(2013, 12, 12),
        AvailableUnits = 0.99
    };

    periods.Add(period);

    var period2 = new AvailabilityPeriod
    {
        AvailableFrom = new DateTime(2013, 12, 12),
        AvailableTo = new DateTime(2015, 12, 12),
        AvailableUnits = 0.94
    };
    periods.Add(period2);
    return periods;
}
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


