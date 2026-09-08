---
title: "Resource.Rates"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Resource 속성. 이 객체에 대한 RateCollection 클래스의 인스턴스를 가져옵니다. 각 항목과 연관된 기간 및 요율의 컬렉션입니다."
type: docs
weight: 640
url: /ko/net/aspose.tasks/resource/rates/
---
## Resource.Rates property

[`RateCollection`](../../ratecollection/) 클래스의 인스턴스를 가져옵니다. 각 항목과 연관된 기간 및 요율의 컬렉션입니다.

```csharp
public RateCollection Rates { get; }
```

## 예제

리소스 요율을 읽는 방법을 보여줍니다.

```csharp
var project = new Project();
var resource = project.Resources.Add();
resource.Set(Rsc.Uid, 1);
resource.Set(Rsc.Name, "Test Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);
resource.Set(Rsc.Work, project.GetDuration(2d, TimeUnitType.Hour));
resource.Set(Rsc.StandardRate, 20m);

var rate1 = resource.Rates.Add(new DateTime(2019, 1, 1, 8, 0, 0));
rate1.RatesTo = new DateTime(2019, 11, 11, 17, 0, 0);
rate1.StandardRate = 5m;
rate1.StandardRateFormat = RateFormatType.Hour;

var rate2 = resource.Rates.Add(new DateTime(2019, 11, 12, 8, 0, 0));
rate2.RatesTo = new DateTime(2019, 12, 31, 17, 0, 0);
rate2.StandardRate = 10m;
rate2.StandardRateFormat = RateFormatType.Hour;

// 요율을 순회합니다
foreach (KeyValuePair<RateType, RateByDateCollection> rate in resource.Rates)
{
    foreach (KeyValuePair<DateTime, Rate> pair in rate.Value)
    {
        Console.WriteLine(pair.Value.RatesFrom);
        Console.WriteLine(pair.Value.RatesTo);
    }
}
```

### 또 보기

* class [RateCollection](../../ratecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


