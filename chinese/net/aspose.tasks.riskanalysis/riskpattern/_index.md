---
title: "类 RiskPattern"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.RiskAnalysis.RiskPattern 类。表示项目任务的风险模式"
type: docs
weight: 1930
url: /zh/net/aspose.tasks.riskanalysis/riskpattern/
---
## RiskPattern class

表示项目任务的风险模式。

```csharp
public class RiskPattern
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [RiskPattern](riskpattern/)(Task) | 初始化 `RiskPattern` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [ConfidenceLevel](../../aspose.tasks.riskanalysis/riskpattern/confidencelevel/) { get; set; } | 获取或设置置信水平，该水平对应实际生成值在乐观和悲观估计范围内出现的时间百分比。默认值为 CL99。 |
| [Distribution](../../aspose.tasks.riskanalysis/riskpattern/distribution/) { get; set; } | 获取或设置 Monte Carlo 仿真中使用的概率分布。默认值为 ProbabilityDistributionType.Normal。 |
| [Optimistic](../../aspose.tasks.riskanalysis/riskpattern/optimistic/) { get; set; } | 获取或设置在最佳项目情景下最可能的任务持续时间的百分比。默认值为 75，这意味着如果估计的任务持续时间为 4 天，则乐观持续时间为 3 天。 |
| [Pessimistic](../../aspose.tasks.riskanalysis/riskpattern/pessimistic/) { get; set; } | 获取或设置在最差项目情景下最可能的任务持续时间的百分比。默认值为 125，这意味着如果估计的任务持续时间为 4 天，则悲观持续时间为 5 天。 |
| [Task](../../aspose.tasks.riskanalysis/riskpattern/task/) { get; } | 获取应用此风险模式的项目任务。 |

## 示例

展示如何定义风险仿真设置。

```csharp
var settings = new RiskAnalysisSettings();
settings.IterationsCount = 200;

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task = project.RootTask.Children.GetById(17);

// 初始化风险模式
var pattern = new RiskPattern(task);

// 为随机数生成器选择一种分布类型以生成可能的值（当前仅支持两种类型，即正态分布和均匀分布）            
// 更多详情请参见此处：https://en.wikipedia.org/wiki/Normal_distribution)
pattern.Distribution = ProbabilityDistributionType.Normal;

// 设置在最佳项目情景下最可能的任务持续时间的百分比 
// 默认值为 75，这意味着如果估计的任务持续时间为 4 天，则乐观持续时间将为 3 天
pattern.Optimistic = 70;

// 设置在最差项目情景下最可能的任务持续时间的百分比 
// 默认值为 125，这意味着如果估计的任务持续时间为 4 天，则悲观持续时间将为 5 天。
pattern.Pessimistic = 130;

// 设置一个置信水平，对应实际值在乐观和悲观估计范围内出现的时间百分比。 
// 可以将其视为标准差的数值：对估计越不确定，随机数生成器使用的标准差值就越大
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

### 另见

* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


