---
title: "类 RiskAnalyzer"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.RiskAnalysis.RiskAnalyzer 类。基于指定的风险分析设置执行蒙特卡罗模拟"
type: docs
weight: 1890
url: /zh/net/aspose.tasks.riskanalysis/riskanalyzer/
---
## RiskAnalyzer class

基于指定的风险分析设置执行蒙特卡罗模拟。

```csharp
public class RiskAnalyzer
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [RiskAnalyzer](riskanalyzer/)(RiskAnalysisSettings) | 初始化 `RiskAnalyzer` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Settings](../../aspose.tasks.riskanalysis/riskanalyzer/settings/) { get; set; } | 获取或设置 [`RiskAnalysisSettings`](../riskanalysissettings/) 类的实例，该实例定义风险分析所需的设置。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Analyze](../../aspose.tasks.riskanalysis/riskanalyzer/analyze/)(Project) | 对指定项目执行风险分析。该分析基于蒙特卡罗模拟，结果是 [`RiskAnalysisResult`](../riskanalysisresult/) 类的实例。 |

## 示例

展示如何通过使用 &lt;see cref=\"Aspose.Tasks.RiskAnalysis.RiskAnalysisSettings\" /&gt; 开始风险分析。

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

// 分析项目风险
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

// 更改设置
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

### 另见

* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


