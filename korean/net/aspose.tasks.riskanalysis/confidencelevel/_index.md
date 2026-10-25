---
title: "열거형 ConfidenceLevel"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.RiskAnalysis.ConfidenceLevel 열거형. 위험 분석에 사용되는 지원되는 신뢰 수준을 지정하며, 이는 실제 값이 낙관적 및 비관적 추정치 내에 있을 확률(백분율)과 대응됩니다."
type: docs
weight: 1850
url: /ko/net/aspose.tasks.riskanalysis/confidencelevel/
---
## ConfidenceLevel enumeration

위험 분석에서 사용되는 지원되는 신뢰 수준을 지정합니다. 이는 실제 값이 낙관적 및 비관적 추정치 범위 내에 있을 확률을 백분율로 나타냅니다.

```csharp
public enum ConfidenceLevel
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| CL99 | `99` | 99 % 신뢰 수준. |
| CL95 | `95` | 95 % 신뢰 수준. |
| CL90 | `90` | 90 % 신뢰 수준. |
| CL85 | `85` | 85 % 신뢰 수준. |
| CL75 | `75` | 75 % 신뢰 수준. |

## 예제

위험 분석을 시작하는 방법을 <see cref=\"Aspose.Tasks.RiskAnalysis.RiskAnalysisSettings\" />를 사용하여 보여줍니다.

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
var earlyFinish = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Expected value: {0}", earlyFinish.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", earlyFinish.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", earlyFinish.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", earlyFinish.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", earlyFinish.GetPercentile(90));
Console.WriteLine("Minimum: {0}", earlyFinish.Minimum);
Console.WriteLine("Maximum: {0}", earlyFinish.Maximum);

settings = new RiskAnalysisSettings
{
    IterationsCount = 300
};

// 설정 변경
analyzer.Settings = settings;

analysisResult = analyzer.Analyze(project);
earlyFinish = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Expected value: {0}", earlyFinish.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", earlyFinish.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", earlyFinish.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", earlyFinish.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", earlyFinish.GetPercentile(90));
Console.WriteLine("Minimum: {0}", earlyFinish.Minimum);
Console.WriteLine("Maximum: {0}", earlyFinish.Maximum);

analysisResult.SaveReport(OutDir + "AnalysisReport_out.pdf");
```

### 또 보기

* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


