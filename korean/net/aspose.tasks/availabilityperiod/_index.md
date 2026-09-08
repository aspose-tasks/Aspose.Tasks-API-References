---
title: "클래스 AvailabilityPeriod"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.AvailabilityPeriod 클래스. 리소스가 사용 가능한 기간을 나타냅니다."
type: docs
weight: 80
url: /ko/net/aspose.tasks/availabilityperiod/
---
## AvailabilityPeriod class

리소스가 사용 가능한 기간을 나타냅니다.

```csharp
public class AvailabilityPeriod
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [AvailabilityPeriod](availabilityperiod/#constructor)() | `AvailabilityPeriod`의 새 인스턴스를 초기화합니다. |
| [AvailabilityPeriod](availabilityperiod/#constructor_1)(DateTime, DateTime, double) | 지정된 날짜 범위와 사용 가능한 단위로 `AvailabilityPeriod`의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [AvailableFrom](../../aspose.tasks/availabilityperiod/availablefrom/) { get; set; } | 지정된 기간 동안 리소스가 사용 가능해지는 날짜를 가져오거나 설정합니다. |
| [AvailableTo](../../aspose.tasks/availabilityperiod/availableto/) { get; set; } | 지정된 기간 동안 리소스가 사용 가능한 마지막 날짜를 가져오거나 설정합니다. |
| [AvailableUnits](../../aspose.tasks/availabilityperiod/availableunits/) { get; set; } | 지정된 기간 동안 리소스가 사용 가능한 비율을 가져오거나 설정합니다. |

## 예제

리소스에 대한 사용 가능 기간을 만드는 방법을 보여줍니다.

```csharp
public void WorkWithAvailabilityPeriod()
{
    var project = new Project();
    var resource = project.Resources.Add("Work Resource");

    // 새 리소스에 사용 가능 기간을 추가합니다
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

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


