---
title: Enum ReportType
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.ReportType enum. Type of the projects graphical report
type: docs
weight: 3300
url: /net/aspose.tasks.visualization/reporttype/
---
## ReportType enumeration

Type of the project's graphical report.

```csharp
public enum ReportType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| ProjectOverview | `0` | Shows the project’s start and finish date, percentage of duration that’s complete, percentage complete for top-level tasks and coming up milestones. |
| CostOverview | `1` | Shows the project’s start and finish dates, the current scheduled and remaining cost, % Complete and cost values for top-level tasks. |
| WorkOverview | `2` | Shows baseline, actual, remaining work for each top-level task and work for work resources. |
| ResourceOverview | `3` | Shows baseline, actual, and remaining work by resource. |
| ResourceCostOverview | `4` | Shows baseline, actual, and remaining cost by resource. |
| CriticalTasks | `5` | Shows project tasks that are critical. |
| LateTasks | `6` | Shows project tasks that are late. |
| Milestones | `7` | Shows milestones that are late, coming up and completed. |
| UpcomingTask | `8` | Shows tasks that are due during the current week and tasks starting during current week. |
| CostOverruns | `9` | Shows cost variance by task and resource. |
| TaskCostOverview | `10` | Shows baseline, actual, and remaining cost of all top-level tasks. |
| OverallocatedResources | `11` | Shows the number of remaining work hours for over allocated resources. |
| SlippingTasks | `12` | Shows tasks that are due to finish after their baseline finish dates (baseline must be set). |
| BestPracticeAnalyzer | `13` | Shows tasks with no actual work, not assigned tasks, tasks with duration less than 8 hours and summaries assigned with the resources. |
| Burndown | `14` | Includes work burndown and task burndown charts. The work burndown chart shows how much work people have finished, how much is scheduled to be finished before the project finish date, and the baseline estimate of how much work would be completed at this point in the project. The task burndown chart shows the number of tasks finished, the number remaining, and the baseline estimate of how many would be finished at this point in the project. |
| CashFlow | `15` | Shows the costs and cumulative costs per quarter for all top-level tasks. |

## Examples

Shows how to save the project burndown report in PDF format to the specified stream.

```csharp
var project = new Project(DataDir + @"Homemoveplan.mpp");
using (var stream = new FileStream(OutDir + "Burndown_out.pdf", FileMode.Create))
{
    project.SaveReport(stream, ReportType.Burndown);
}
```

### See Also

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


