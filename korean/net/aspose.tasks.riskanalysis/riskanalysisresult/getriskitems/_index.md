---
title: "RiskAnalysisResult.GetRiskItems"
second_title: "Aspose.Tasks for .NET API 참조"
description: "RiskAnalysisResult 메서드. 지정된 위험 유형에 대한 RiskItemStatisticsCollection의 인스턴스를 반환합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks.riskanalysis/riskanalysisresult/getriskitems/
---
## RiskAnalysisResult.GetRiskItems method

지정된 위험 유형에 대한 [`RiskItemStatisticsCollection`](../../riskitemstatisticscollection/) 인스턴스를 반환합니다.

```csharp
public RiskItemStatisticsCollection GetRiskItems(RiskItemType itemType)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| itemType | RiskItemType | 지정된 위험 유형; [`RiskItemType`](../../riskitemtype/) 열거형의 값 중 하나일 수 있습니다. |

### 반환 값

지정된 위험 유형에 대한 [`RiskItemStatisticsCollection`](../../riskitemstatisticscollection/) 인스턴스.

## 예제

위험 통계를 계산하고 PDF 보고서로 저장하는 방법을 보여줍니다.

```csharp
var settings = new RiskAnalysisSettings
{
    IterationsCount = 200
};

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task = project.RootTask.Children.GetById(17);

// 위험 패턴을 초기화합니다.
var pattern = new RiskPattern(task)
{
    // 무작위 숫자 생성기가 가능한 값을 생성하도록 분포 유형을 선택합니다 (현재 지원되는 두 가지 유형은 정규 분포와 균등 분포뿐입니다).
    // 자세한 내용은 여기에서 확인하십시오: https://en.wikipedia.org/wiki/Normal_distribution)
    Distribution = ProbabilityDistributionType.Normal,

    // 최상의 프로젝트 시나리오에서 발생할 수 있는 가장 가능성이 높은 작업 기간의 백분율을 설정합니다.
    // 기본값은 75이며, 이는 지정된 작업 기간이 4일로 추정될 경우 낙관적인 기간은 3일이 됨을 의미합니다.
    Optimistic = 70,

    // 최악의 프로젝트 시나리오에서 발생할 수 있는 가장 가능성이 높은 작업 기간의 백분율을 설정합니다.
    // 기본값은 125이며, 이는 지정된 작업 기간이 4일로 추정될 경우 비관적인 기간은 5일이 됨을 의미합니다.
    Pessimistic = 130,

    // 실제 값이 낙관적 및 비관적 추정치 사이에 있을 확률에 해당하는 신뢰 수준을 설정합니다.
    // 이를 표준 편차 값으로 생각할 수 있습니다: 추정이 불확실할수록 무작위 숫자 생성기에 사용되는 표준 편차 값이 커집니다.
    ConfidenceLevel = ConfidenceLevel.CL75
};
settings.Patterns.Add(pattern);

// 프로젝트 위험을 분석합니다.
var analyzer = new RiskAnalyzer(settings);
var analysisResult = analyzer.Analyze(project);

// 파일 경로를 사용하여 분석을 보고서 파일로 저장합니다.
analysisResult.SaveReport(OutDir + "AnalysisResult_out.pdf");

// 또는 분석을 스트림에 저장합니다.
using (var stream = new FileStream(OutDir + "AnalysisResult_out1.pdf", FileMode.Create))
{
    analysisResult.SaveReport(stream);
}
```

### 또 보기

* class [RiskItemStatisticsCollection](../../riskitemstatisticscollection/)
* enum [RiskItemType](../../riskitemtype/)
* class [RiskAnalysisResult](../)
* namespace [Aspose.Tasks.RiskAnalysis](../../riskanalysisresult/)
* assembly [Aspose.Tasks](../../../)


