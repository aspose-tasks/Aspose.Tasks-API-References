---
title: "RiskPattern"
second_title: "适用于 Python via .NET 的 Aspose.Tasks API 参考"
description: 
type: docs
weight: 60
url: /zh/python-net/aspose.tasks.riskanalysis/riskpattern/
---

## RiskPattern class

表示项目任务的风险模式。

RiskPattern 类型公开以下成员：
## 构造函数
| 名称 | 描述 |
| :- | :- |
| RiskPattern(task) | 初始化一个新的 [RiskPattern](/tasks/python-net/aspose.tasks.riskanalysis/riskpattern/) 类实例。 |
## 属性
| 名称 | 描述 |
| :- | :- |
| task | 获取此风险模式应用的项目任务。 |
| 分布 | 获取或设置在 Monte Carlo 仿真中使用的概率分布。<br/>            默认值为 ProbabilityDistributionType.Normal。 |
| confidence_level | 获取或设置置信水平，以对应实际生成值在乐观和悲观估计范围内出现的时间百分比。<br/>            默认值为 CL99。 |
| optimistic | 获取或设置在最佳项目情景下最可能的任务持续时间的百分比。<br/>            默认值为 75，这意味着如果估计的任务持续时间为 4 天，则 optimistic 持续时间为 3 天。 |
| pessimistic | 获取或设置在最差项目情景下最可能的任务持续时间的百分比。<br/>            默认值为 125，这意味着如果估计的任务持续时间为 4 天，则 pessimistic 持续时间为 5 天。 |

### 另见

* namespace [aspose.tasks.riskanalysis](/tasks/python-net/aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](/tasks/python-net/)

