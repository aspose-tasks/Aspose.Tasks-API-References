---
title: "Rate.OvertimeRateFormat"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rate 속성. Microsoft Project에서 초과 근무 요금을 표시하는 데 사용되는 단위를 가져오거나 설정합니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks/rate/overtimerateformat/
---
## Rate.OvertimeRateFormat property

Microsoft Project에서 초과 근무 요금을 표시하는 데 사용되는 단위를 가져오거나 설정합니다.

```csharp
public RateFormatType OvertimeRateFormat { get; set; }
```

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

* enum [RateFormatType](../../rateformattype/)
* class [Rate](../)
* namespace [Aspose.Tasks](../../rate/)
* assembly [Aspose.Tasks](../../../)


