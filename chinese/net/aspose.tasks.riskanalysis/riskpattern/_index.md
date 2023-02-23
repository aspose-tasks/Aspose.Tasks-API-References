---
title: Class RiskPattern
second_title: Aspose.Tasks for .NET API 参考
description: Aspose.Tasks.RiskAnalysis.RiskPattern 班级. 表示项目任务的风险模式
type: docs
weight: 1670
url: /zh/net/aspose.tasks.riskanalysis/riskpattern/
---
## RiskPattern class

表示项目任务的风险模式。

```csharp
public class RiskPattern
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [RiskPattern](riskpattern/)(Task) | 初始化一个新的实例`RiskPattern`类. |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [ConfidenceLevel](../../aspose.tasks.riskanalysis/riskpattern/confidencelevel/) { get; set; } | 获取或设置与实际生成的值在乐观和悲观估计范围内的时间百分比相对应的置信度。 默认值为 CL99. |
| [Distribution](../../aspose.tasks.riskanalysis/riskpattern/distribution/) { get; set; } | 获取或设置蒙特卡洛模拟中使用的概率分布。 默认值为 ProbabilityDistributionType.Normal. |
| [Optimistic](../../aspose.tasks.riskanalysis/riskpattern/optimistic/) { get; set; } | 获取或设置最可能发生的任务持续时间的百分比，它可能发生在最佳项目场景中。 默认值为 75，这意味着如果估计的指定任务持续时间为 4 天，则乐观持续时间将为 3 天。 |
| [Pessimistic](../../aspose.tasks.riskanalysis/riskpattern/pessimistic/) { get; set; } | 获取或设置在最坏可能的项目场景下最有可能发生的任务持续时间的百分比。 默认值为 125，这意味着如果估计指定任务持续时间为 4 天，那么悲观持续时间将为 5 天。 |
| [Task](../../aspose.tasks.riskanalysis/riskpattern/task/) { get; } | 获取应用此风险模式的项目任务。 |

### 也可以看看

* 命名空间 [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* 部件 [Aspose.Tasks](../../)


