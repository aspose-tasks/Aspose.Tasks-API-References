---
title: "类 RiskAnalysisSettings"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.RiskAnalysis.RiskAnalysisSettings 类。指定执行风险分析的设置"
type: docs
weight: 1880
url: /zh/net/aspose.tasks.riskanalysis/riskanalysissettings/
---
## RiskAnalysisSettings class

指定执行风险分析的设置。

```csharp
public class RiskAnalysisSettings
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [RiskAnalysisSettings](riskanalysissettings/)() | 初始化 `RiskAnalysisSettings` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [IterationsCount](../../aspose.tasks.riskanalysis/riskanalysissettings/iterationscount/) { get; set; } | 获取或设置蒙特卡罗模拟中使用的迭代次数。默认值为 100。 |
| [Patterns](../../aspose.tasks.riskanalysis/riskanalysissettings/patterns/) { get; } | 获取包含 [`RiskPattern`](../riskpattern/) 类实例的集合。 |

## 示例

展示如何为蒙特卡罗模拟准备风险分析设置。

```csharp
var riskAnalysisSettings = new RiskAnalysisSettings();

// 设置 Monte Carlo 仿真的迭代次数（默认值为 100）。
riskAnalysisSettings.IterationsCount = 200;

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

riskAnalysisSettings.Patterns.Add(pattern);

var analyzer = new RiskAnalyzer(riskAnalysisSettings);
var analysisResult = analyzer.Analyze(project);
var rootEarlyFinish = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Expected value: {0}", rootEarlyFinish.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", rootEarlyFinish.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", rootEarlyFinish.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", rootEarlyFinish.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", rootEarlyFinish.GetPercentile(90));
Console.WriteLine("Minimum: {0}", rootEarlyFinish.Minimum);
Console.WriteLine("Maximum: {0}", rootEarlyFinish.Maximum);

analysisResult.SaveReport(OutDir + "AnalysisReport_out.pdf");
```

### 另见

* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


