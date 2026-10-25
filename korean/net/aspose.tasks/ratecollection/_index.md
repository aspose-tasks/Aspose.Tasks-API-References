---
title: "클래스 RateCollection"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.RateCollection 클래스. Rate 객체를 포함하는 컬렉션을 나타냅니다."
type: docs
weight: 1630
url: /ko/net/aspose.tasks/ratecollection/
---
## RateCollection class

`[`Rate`](../rate/)` 객체를 포함하는 컬렉션을 나타냅니다.

```csharp
public class RateCollection : IDictionary<RateType, RateByDateCollection>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Count](../../aspose.tasks/ratecollection/count/) { get; } | RateCollection에 포함된 요소 수를 가져옵니다. |
| [IsReadOnly](../../aspose.tasks/ratecollection/isreadonly/) { get; } | 이 컬렉션이 읽기 전용인지 여부를 나타내는 값을 가져옵니다. |
| [Item](../../aspose.tasks/ratecollection/item/) { get; set; } | 지정된 인덱스에 있는 요소를 반환하거나 설정합니다. |
| [ParentResource](../../aspose.tasks/ratecollection/parentresource/) { get; } | 이 컬렉션에 대한 상위 [`Resource`](../resource/) 객체를 가져옵니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Add](../../aspose.tasks/ratecollection/add/#add)(DateTime) | 새로운 [`Rate`](../rate/) 인스턴스를 이 컬렉션에 추가합니다. |
| [Add](../../aspose.tasks/ratecollection/add/#add_1)(DateTime, RateType) | 새로운 [`Rate`](../rate/) 인스턴스를 이 컬렉션에 추가합니다. |
| [GetEnumerator](../../aspose.tasks/ratecollection/getenumerator/)() | 이 컬렉션에 대한 열거자를 반환합니다. |
| [Remove](../../aspose.tasks/ratecollection/remove/)(Rate) | 이 컬렉션에서 Rate 인스턴스를 제거합니다. |
| [ToList](../../aspose.tasks/ratecollection/tolist/#tolist)() | `RateCollection` 객체를 [`Rate`](../rate/) 객체 목록으로 변환합니다. |
| [ToList](../../aspose.tasks/ratecollection/tolist/#tolist_1)(RateType) | `RateCollection` 객체를 지정된 [`RateType`](../ratetype/) 유형으로 필터링된 [`Rate`](../rate/) 객체 목록으로 변환합니다. |

## 예제

요금 컬렉션을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var resource = project.Resources.Add("Test Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);
resource.Set(Rsc.Work, project.GetDuration(2d, TimeUnitType.Hour));
resource.Set(Rsc.StandardRate, 20m);

var rate1 = resource.Rates.Add(new DateTime(2019, 1, 1, 8, 0, 0));
rate1.RatesTo = new DateTime(2019, 11, 11, 17, 0, 0);
rate1.StandardRate = 5m;
rate1.StandardRateFormat = RateFormatType.Hour;

var rate2 = resource.Rates.Add(new DateTime(2019, 11, 12, 8, 0, 0), RateType.B);
rate2.RatesTo = new DateTime(2019, 12, 31, 17, 0, 0);
rate2.StandardRate = 10m;
rate2.StandardRateFormat = RateFormatType.Hour;

Console.WriteLine("Print rates of '{0}' resource: ", resource.Rates.ParentResource.Get(Rsc.Name));
Console.WriteLine("Count of rates: {0}", resource.Rates.Count);
Console.WriteLine("Is rate collection read-only: {0}", resource.Rates.IsReadOnly);
foreach (KeyValuePair<RateType, RateByDateCollection> sortedRates in resource.Rates)
{
    foreach (KeyValuePair<DateTime, Rate> pair in sortedRates.Value)
    {
        var rate = pair.Value;
        Console.WriteLine("Rates From: " + rate.RatesFrom);
        Console.WriteLine("Rates To: " + rate.RatesTo);
        Console.WriteLine("Rate Table: " + rate.RateTable);
        Console.WriteLine();
    }
}

// 인덱스 접근으로 최신 요금을 가져옵니다.
var rateToUpdate = resource.Rates[RateType.B][new DateTime(2019, 11, 12, 8, 0, 0)];
rateToUpdate.RatesTo = new DateTime(2020, 12, 31, 17, 0, 0);
Console.WriteLine("Rates From: " + rateToUpdate.RatesFrom);
Console.WriteLine("Rates To: " + rateToUpdate.RatesTo);

// ...
// 요금을 사용합니다.
// ...

// 유형 A의 모든 요금을 제거합니다.
List<Rate> rates = resource.Rates.ToList(RateType.A);
for (var i = 0; i < rates.Count; i++)
{
    var rateToRemove = rates[i];
    resource.Rates.Remove(rateToRemove);
}

// 요금 컬렉션을 평면 목록으로 변환합니다.
Console.WriteLine("Iterate over the rates after remove the A-typed values: ");
List<Rate> list = resource.Rates.ToList();
foreach (var rt in list)
{
    Console.WriteLine("Rates From: " + rt.RatesFrom);
    Console.WriteLine("Rates To: " + rt.RatesTo);
    Console.WriteLine("Rate Table: " + rt.RateTable);
}
```

### 또 보기

* enum [RateType](../ratetype/)
* class [RateByDateCollection](../ratebydatecollection/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


