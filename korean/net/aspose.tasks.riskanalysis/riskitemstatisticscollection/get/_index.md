---
title: "RiskItemStatisticsCollection.Get"
second_title: "Aspose.Tasks for .NET API 참조"
description: "RiskItemStatisticsCollection 메서드. 지정된 Task 객체와 연결된 이 컬렉션에 포함된 RiskItemStatistics 클래스의 인스턴스를 반환합니다. 항목을 찾을 수 없으면 null을 반환합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks.riskanalysis/riskitemstatisticscollection/get/
---
## RiskItemStatisticsCollection.Get method

이 컬렉션에 포함되어 지정된 Task 객체와 연결된 [`RiskItemStatistics`](../../riskitemstatistics/) 클래스의 인스턴스를 반환합니다; 항목을 찾을 수 없으면 null을 반환합니다.

```csharp
public RiskItemStatistics Get(Task task)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| task | Task | 지정된 [`Task`](../../../aspose.tasks/task/) 클래스의 인스턴스. |

### 반환 값

지정된 task 객체와 연결된 위험 항목을 찾으면 반환하고, 그렇지 않으면 null을 반환합니다.

## 예제

위험 통계 컬렉션을 사용하는 방법을 보여줍니다.

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

var analyzer = new RiskAnalyzer(settings);
var analysisResult = analyzer.Analyze(project);

// 모든 통계 항목을 반복합니다.
var statistics = analysisResult.GetRiskItems(RiskItemType.EarlyFinish);

foreach (var statistic in statistics)
{
    Console.WriteLine("Short statistic: " + statistic);
    Console.WriteLine();
    Console.WriteLine("Statistic details: ");
    Console.WriteLine("Item Type: {0}", statistic.ItemType);
    Console.WriteLine("Expected value: {0}", statistic.ExpectedValue);
    Console.WriteLine("StandardDeviation: {0}", statistic.StandardDeviation);
    Console.WriteLine("10% Percentile: {0}", statistic.GetPercentile(10));
    Console.WriteLine("50% Percentile: {0}", statistic.GetPercentile(50));
    Console.WriteLine("90% Percentile: {0}", statistic.GetPercentile(90));
    Console.WriteLine("Minimum: {0}", statistic.Minimum);
    Console.WriteLine("Maximum: {0}", statistic.Maximum);
}

// 또는 특정 통계를 가져옵니다.
var itemStatistics = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Print the specific statistic: ");
Console.WriteLine("Expected value: {0}", itemStatistics.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", itemStatistics.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", itemStatistics.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", itemStatistics.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", itemStatistics.GetPercentile(90));
Console.WriteLine("Minimum: {0}", itemStatistics.Minimum);
Console.WriteLine("Maximum: {0}", itemStatistics.Maximum);
```

### 또 보기

* class [RiskItemStatistics](../../riskitemstatistics/)
* class [Task](../../../aspose.tasks/task/)
* class [RiskItemStatisticsCollection](../)
* namespace [Aspose.Tasks.RiskAnalysis](../../riskitemstatisticscollection/)
* assembly [Aspose.Tasks](../../../)


