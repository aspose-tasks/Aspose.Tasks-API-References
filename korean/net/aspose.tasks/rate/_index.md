---
title: "클래스 Rate"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Rate 클래스. 해당 기간 동안 리소스에 적용되는 시간 기간 및 요금 정의를 나타냅니다."
type: docs
weight: 1610
url: /ko/net/aspose.tasks/rate/
---
## Rate class

해당 기간 동안 리소스에 적용되는 시간 기간 및 요율 정의를 나타냅니다.

```csharp
public class Rate
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [CostPerUse](../../aspose.tasks/rate/costperuse/) { get; set; } | 리소스 사용당 비용을 가져오거나 설정합니다. 리소스에 요금표가 존재하는 경우 현재 날짜에서 이 값을 가져옵니다. |
| [OvertimeRate](../../aspose.tasks/rate/overtimerate/) { get; set; } | 리소스의 시간당 초과 근무 요금을 가져오거나 설정합니다. |
| [OvertimeRateFormat](../../aspose.tasks/rate/overtimerateformat/) { get; set; } | Microsoft Project에서 초과 근무 요금을 표시하는 데 사용되는 단위를 가져오거나 설정합니다. |
| [RatesFrom](../../aspose.tasks/rate/ratesfrom/) { get; set; } | 요금이 적용되는 날짜를 가져오거나 설정합니다. |
| [RatesTo](../../aspose.tasks/rate/ratesto/) { get; set; } | 요금이 유효한 마지막 날짜를 가져오거나 설정합니다. |
| [RateTable](../../aspose.tasks/rate/ratetable/) { get; set; } | 리소스에 대한 요금표의 고유 식별자를 가져오거나 설정합니다. |
| [StandardRate](../../aspose.tasks/rate/standardrate/) { get; set; } | 리소스의 시간당 표준 요금을 가져오거나 설정합니다. |
| [StandardRateFormat](../../aspose.tasks/rate/standardrateformat/) { get; set; } | Microsoft Project에서 표준 요금을 표시하는 데 사용되는 단위를 가져오거나 설정합니다. |

## 예제

리소스 요금을 사용하는 방법을 보여줍니다.

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

// 프로젝트와 작업...
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


