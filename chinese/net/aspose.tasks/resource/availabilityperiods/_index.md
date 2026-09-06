---
title: "Resource.AvailabilityPeriods"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Resource 属性。获取 AvailabilityPeriodCollection 类的实例。该集合包含资源可用的期间。"
type: docs
weight: 130
url: /zh/net/aspose.tasks/resource/availabilityperiods/
---
## Resource.AvailabilityPeriods property

获取 [`AvailabilityPeriodCollection`](../../availabilityperiodcollection/) 类的实例。该集合包含资源可用的期间。

```csharp
public AvailabilityPeriodCollection AvailabilityPeriods { get; }
```

## 示例

展示如何为资源添加可用期间。

```csharp
var project = new Project();
var resource = project.Resources.Add("Resource");

var availabilityPeriod = new AvailabilityPeriod
{
    AvailableFrom = new DateTime(2020, 4, 1, 8, 0, 0),
    AvailableTo = new DateTime(2020, 4, 1, 17, 0, 0),
    AvailableUnits = 2d
};
resource.AvailabilityPeriods.Add(availabilityPeriod);

var availabilityPeriod2 = new AvailabilityPeriod
{
    AvailableFrom = new DateTime(2020, 4, 2, 8, 0, 0),
    AvailableTo = new DateTime(2020, 4, 2, 17, 0, 0),
    AvailableUnits = 3d
};
resource.AvailabilityPeriods.Add(availabilityPeriod2);
```

### 另见

* class [AvailabilityPeriodCollection](../../availabilityperiodcollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


