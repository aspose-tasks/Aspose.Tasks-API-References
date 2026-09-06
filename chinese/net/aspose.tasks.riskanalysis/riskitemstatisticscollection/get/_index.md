---
title: "RiskItemStatisticsCollection.Get"
second_title: "Aspose.Tasks for .NET API 参考"
description: "RiskItemStatisticsCollection 方法。返回一个 RiskItemStatistics 类的实例，该实例包含在此集合中并与指定的 Task 对象关联，如果未找到该项则为 null。"
type: docs
weight: 10
url: /zh/net/aspose.tasks.riskanalysis/riskitemstatisticscollection/get/
---
## RiskItemStatisticsCollection.Get method

返回一个 [`RiskItemStatistics`](../../riskitemstatistics/) 类的实例，该实例包含在此集合中并与指定的 Task 对象关联；如果未找到该项则为 null。

```csharp
public RiskItemStatistics Get(Task task)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| task | Task | 指定的 [`Task`](../../../aspose.tasks/task/) 类的实例。 |

### 返回值

如果找到，则为与指定任务对象关联的风险项；否则为 null。

## 示例

展示如何使用风险统计集合。

```csharp
var settings = new RiskAnalysisSettings
{
    IterationsCount = 200
};

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task = project.RootTask.Children.GetById(17);

// 初始化风险模式
var pattern = new RiskPattern(task)
{
    // 为随机数生成器选择一种分布类型以生成可能的值（当前仅支持两种类型，即正态分布和均匀分布）            
    // 更多详情请参见此处：https://en.wikipedia.org/wiki/Normal_distribution)
    Distribution = ProbabilityDistributionType.Normal,

    // 设置在最佳项目情景下最可能的任务持续时间的百分比 
    // 默认值为 75，这意味着如果估计的任务持续时间为 4 天，则乐观持续时间将为 3 天
    Optimistic = 70,

    // 设置在最差项目情景下最可能的任务持续时间的百分比 
    // 默认值为 125，这意味着如果估计的任务持续时间为 4 天，则悲观持续时间将为 5 天。
    Pessimistic = 130,

    // 设置一个置信水平，对应实际值在乐观和悲观估计范围内出现的时间百分比。 
    // 可以将其视为标准差的数值：对估计越不确定，随机数生成器使用的标准差值就越大
    ConfidenceLevel = ConfidenceLevel.CL75
};
settings.Patterns.Add(pattern);

var analyzer = new RiskAnalyzer(settings);
var analysisResult = analyzer.Analyze(project);

// 遍历所有统计项
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

// 或获取特定统计信息
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

### 另见

* class [RiskItemStatistics](../../riskitemstatistics/)
* class [Task](../../../aspose.tasks/task/)
* class [RiskItemStatisticsCollection](../)
* namespace [Aspose.Tasks.RiskAnalysis](../../riskitemstatisticscollection/)
* assembly [Aspose.Tasks](../../../)


