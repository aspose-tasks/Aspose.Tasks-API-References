---
title: "클래스 RiskPattern"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.RiskAnalysis.RiskPattern 클래스. 프로젝트 작업에 대한 위험 패턴을 나타냅니다."
type: docs
weight: 1930
url: /ko/net/aspose.tasks.riskanalysis/riskpattern/
---
## RiskPattern class

프로젝트 작업에 대한 위험 패턴을 나타냅니다.

```csharp
public class RiskPattern
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [RiskPattern](riskpattern/)(Task) | `RiskPattern` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [ConfidenceLevel](../../aspose.tasks.riskanalysis/riskpattern/confidencelevel/) { get; set; } | 실제 생성된 값이 낙관적 및 비관적 추정치 범위 내에 있을 확률에 해당하는 신뢰 수준을 가져오거나 설정합니다. 기본값은 CL99입니다. |
| [Distribution](../../aspose.tasks.riskanalysis/riskpattern/distribution/) { get; set; } | 몬테카를로 시뮬레이션에 사용되는 확률 분포를 가져오거나 설정합니다. 기본값은 ProbabilityDistributionType.Normal입니다. |
| [Optimistic](../../aspose.tasks.riskanalysis/riskpattern/optimistic/) { get; set; } | 가능한 최상의 프로젝트 시나리오에서 발생할 수 있는 가장 가능성 높은 작업 기간의 비율을 가져오거나 설정합니다. 기본값은 75이며, 이는 지정된 작업 기간이 4일로 추정될 경우 낙관적 기간은 3일이 된다는 의미입니다. |
| [Pessimistic](../../aspose.tasks.riskanalysis/riskpattern/pessimistic/) { get; set; } | 가능한 최악의 프로젝트 시나리오에서 발생할 수 있는 가장 가능성 높은 작업 기간의 비율을 가져오거나 설정합니다. 기본값은 125이며, 이는 지정된 작업 기간이 4일로 추정될 경우 비관적 기간은 5일이 된다는 의미입니다. |
| [Task](../../aspose.tasks.riskanalysis/riskpattern/task/) { get; } | 이 위험 패턴이 적용되는 프로젝트 작업을 가져옵니다. |

## 예제

위험 시뮬레이션 설정을 정의하는 방법을 보여줍니다.

```csharp
var settings = new RiskAnalysisSettings();
settings.IterationsCount = 200;

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task = project.RootTask.Children.GetById(17);

// 위험 패턴을 초기화합니다.
var pattern = new RiskPattern(task);

// 무작위 숫자 생성기가 가능한 값을 생성하도록 분포 유형을 선택합니다 (현재 지원되는 두 가지 유형은 정규 분포와 균등 분포뿐입니다).
// 자세한 내용은 여기에서 확인하십시오: https://en.wikipedia.org/wiki/Normal_distribution)
pattern.Distribution = ProbabilityDistributionType.Normal;

// 최상의 프로젝트 시나리오에서 발생할 수 있는 가장 가능성이 높은 작업 기간의 백분율을 설정합니다.
// 기본값은 75이며, 이는 지정된 작업 기간이 4일로 추정될 경우 낙관적인 기간은 3일이 됨을 의미합니다.
pattern.Optimistic = 70;

// 최악의 프로젝트 시나리오에서 발생할 수 있는 가장 가능성이 높은 작업 기간의 백분율을 설정합니다.
// 기본값은 125이며, 이는 지정된 작업 기간이 4일로 추정될 경우 비관적인 기간은 5일이 됨을 의미합니다.
pattern.Pessimistic = 130;

// 실제 값이 낙관적 및 비관적 추정치 사이에 있을 확률에 해당하는 신뢰 수준을 설정합니다.
// 이를 표준 편차 값으로 생각할 수 있습니다: 추정이 불확실할수록 무작위 숫자 생성기에 사용되는 표준 편차 값이 커집니다.
pattern.ConfidenceLevel = ConfidenceLevel.CL75;

settings.Patterns.Add(pattern);

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

analysisResult.SaveReport(OutDir + "AnalysisReport_out.pdf");
```

### 또 보기

* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


