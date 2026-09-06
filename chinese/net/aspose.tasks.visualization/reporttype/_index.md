---
title: "枚举 ReportType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Visualization.ReportType 枚举。项目图形报告的类型"
type: docs
weight: 3330
url: /zh/net/aspose.tasks.visualization/reporttype/
---
## ReportType enumeration

项目图形报告的类型。

```csharp
public enum ReportType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| ProjectOverview | `0` | 显示项目的开始和结束日期、已完成的持续时间百分比、顶层任务的完成百分比以及即将到来的里程碑。 |
| CostOverview | `1` | 显示项目的开始和结束日期、当前计划和剩余成本、完成百分比以及顶层任务的成本值。 |
| WorkOverview | `2` | 显示每个顶层任务的基线、实际和剩余工作以及工作资源的工作量。 |
| ResourceOverview | `3` | 按资源显示基线、实际和剩余工作。 |
| ResourceCostOverview | `4` | 按资源显示基线、实际和剩余成本。 |
| CriticalTasks | `5` | 显示关键的项目任务。 |
| LateTasks | `6` | 显示逾期的项目任务。 |
| Milestones | `7` | 显示逾期、即将到来和已完成的里程碑。 |
| UpcomingTask | `8` | 显示本周到期的任务以及本周开始的任务。 |
| CostOverruns | `9` | 按任务和资源显示成本差异。 |
| TaskCostOverview | `10` | 显示所有顶层任务的基线、实际和剩余成本。 |
| OverallocatedResources | `11` | 显示超额分配资源的剩余工作小时数。 |
| SlippingTasks | `12` | 显示计划在基线完成日期之后完成的任务（必须设置基线）。 |
| BestPracticeAnalyzer | `13` | 显示没有实际工作、未分配的任务、持续时间少于8小时的任务以及已分配资源的汇总任务。 |
| Burndown | `14` | 包括工作燃尽图和任务燃尽图。工作燃尽图显示人员已完成的工作量、在项目结束日期前计划完成的工作量，以及基线估计的此时项目应完成的工作量。任务燃尽图显示已完成的任务数量、剩余任务数量，以及基线估计的此时应完成的任务数量。 |
| CashFlow | `15` | 显示所有顶层任务的每季度成本和累计成本。 |

## 示例

展示如何将项目燃尽报告以 PDF 格式保存到指定的流中。

```csharp
var project = new Project(DataDir + @"Homemoveplan.mpp");
using (var stream = new FileStream(OutDir + "Burndown_out.pdf", FileMode.Create))
{
    project.SaveReport(stream, ReportType.Burndown);
}
```

### 另见

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


