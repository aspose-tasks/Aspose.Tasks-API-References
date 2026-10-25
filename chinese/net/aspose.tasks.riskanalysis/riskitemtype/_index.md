---
title: "枚举 RiskItemType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.RiskAnalysis.RiskItemType 枚举。指定在风险分析期间收集统计信息的任务字段"
type: docs
weight: 1920
url: /zh/net/aspose.tasks.riskanalysis/riskitemtype/
---
## RiskItemType enumeration

指定在风险分析期间收集统计信息的任务字段。

```csharp
public enum RiskItemType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Start | `0` | 任务开始。 |
| Finish | `1` | 任务完成。 |
| EarlyStart | `2` | 任务提前开始。 |
| EarlyFinish | `3` | 任务提前完成。 |
| LateStart | `4` | 任务延迟开始。 |
| LateFinish | `5` | 任务延迟完成。 |

## 示例

展示如何计算风险统计并将其保存为 PDF 报告。

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

// 将分析保存为报告到文件路径指定的文件中
analysisResult.SaveReport(OutDir + "AnalysisResult_out.pdf");

// 或将分析保存到流中
using (var stream = new FileStream(OutDir + "AnalysisResult_out1.pdf", FileMode.Create))
{
    analysisResult.SaveReport(stream);
}
```

### 另见

* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


