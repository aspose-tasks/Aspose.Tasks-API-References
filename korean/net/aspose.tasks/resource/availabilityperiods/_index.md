---
title: "Resource.AvailabilityPeriods"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Resource 속성. AvailabilityPeriodCollection 클래스의 인스턴스를 가져옵니다. 리소스가 사용 가능한 기간들의 컬렉션입니다."
type: docs
weight: 130
url: /ko/net/aspose.tasks/resource/availabilityperiods/
---
## Resource.AvailabilityPeriods property

[`AvailabilityPeriodCollection`](../../availabilityperiodcollection/) 클래스의 인스턴스를 가져옵니다. 리소스가 사용 가능한 기간들의 컬렉션입니다.

```csharp
public AvailabilityPeriodCollection AvailabilityPeriods { get; }
```

## 예제

리소스에 가용 기간을 추가하는 방법을 보여줍니다.

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

### 또 보기

* class [AvailabilityPeriodCollection](../../availabilityperiodcollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


