---
title: "클래스 RiskAnalyzer"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.RiskAnalysis.RiskAnalyzer 클래스. 지정된 위험 분석 설정을 기반으로 몬테카를로 시뮬레이션을 수행합니다."
type: docs
weight: 1890
url: /ko/net/aspose.tasks.riskanalysis/riskanalyzer/
---
## RiskAnalyzer class

지정된 위험 분석 설정을 기반으로 몬테카를로 시뮬레이션을 수행합니다.

```csharp
public class RiskAnalyzer
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [RiskAnalyzer](riskanalyzer/)(RiskAnalysisSettings) | 새 `RiskAnalyzer` 클래스 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Settings](../../aspose.tasks.riskanalysis/riskanalyzer/settings/) { get; set; } | 위험 분석에 필요한 설정을 정의하는 [`RiskAnalysisSettings`](../riskanalysissettings/) 클래스 인스턴스를 가져오거나 설정합니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Analyze](../../aspose.tasks.riskanalysis/riskanalyzer/analyze/)(Project) | 지정된 프로젝트에 대한 위험 분석을 수행합니다. 분석은 몬테카를로 시뮬레이션을 기반으로 하며 결과는 [`RiskAnalysisResult`](../riskanalysisresult/) 클래스의 인스턴스입니다. |

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


