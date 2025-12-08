---
title: Enum TaskUsageViewField
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.TaskUsageViewField enum. Represents possible fields in TaskUsageView object
type: docs
weight: 2440
url: /net/aspose.tasks/taskusageviewfield/
---
## TaskUsageViewField enumeration

Represents possible fields in [`TaskUsageView`](../taskusageview/) object.

```csharp
public enum TaskUsageViewField
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Undefined | `-1` | Indicates Undefined task usage view field. |
| Work | `0` | Indicates Work task usage view field. |
| OvertimeWork | `1` | Indicates Overtime Work task usage view field. |
| ActualWork | `2` | Indicates Actual Work task usage view field. |
| ActualOvertimeWork | `3` | Indicates Actual Overtime Work task usage view field. |
| CumulativeWork | `4` | Indicates Cumulative Work task usage view field. |
| BaselineWork | `5` | Indicates Baseline Work task usage view field. |
| Overallocation | `6` | Indicates Overallocation task usage view field. |
| PercentAllocation | `7` | Indicates Percent Allocation task usage view field. |
| PeakUnits | `8` | Indicates Peak Units task usage view field. |
| Cost | `9` | Indicates Cost task usage view field. |
| FixedCost | `10` | Indicates Fixed Cost task usage view field. |
| ActualCost | `11` | Indicates Actual Cost task usage view field. |
| BaselineCost | `12` | Indicates Baseline Cost task usage view field. |
| CumulativeCost | `13` | Indicates Cumulative Cost task usage view field. |
| BCWS | `14` | Indicates BCWS task usage view field. |
| BCWP | `15` | Indicates BCWP task usage view field. |
| ACWP | `16` | Indicates ACWP task usage view field. |
| SV | `17` | Indicates SV task usage view field. |
| CV | `18` | Indicates CV task usage view field. |
| RegularWork | `19` | Indicates Regular Work task usage view field. |
| PercentComplete | `20` | Indicates Percent Complete task usage view field. |
| CumulativePercentComplete | `21` | Indicates Cumulative Percent Complete task usage view field. |
| Baseline1Work | `22` | Indicates Baseline1 Work task usage view field. |
| Baseline1Cost | `23` | Indicates Baseline1 Cost task usage view field. |
| Baseline2Work | `24` | Indicates Baseline2 Work task usage view field. |
| Baseline2Cost | `25` | Indicates Baseline2 Cost task usage view field. |
| Baseline3Work | `26` | Indicates Baseline3 Work task usage view field. |
| Baseline3Cost | `27` | Indicates Baseline3 Cost task usage view field. |
| Baseline4Work | `28` | Indicates Baseline4 Work task usage view field. |
| Baseline4Cost | `29` | Indicates Baseline4 Cost task usage view field. |
| Baseline5Work | `30` | Indicates Baseline5 Work task usage view field. |
| Baseline5Cost | `31` | Indicates Baseline5 Cost task usage view field. |
| Baseline6Work | `32` | Indicates Baseline6 Work task usage view field. |
| Baseline6Cost | `33` | Indicates Baseline6 Cost task usage view field. |
| Baseline7Work | `34` | Indicates Baseline7 Work task usage view field. |
| Baseline7Cost | `35` | Indicates Baseline7 Cost task usage view field. |
| Baseline8Work | `36` | Indicates Baseline8 Work task usage view field. |
| Baseline8Cost | `37` | Indicates Baseline8 Cost task usage view field. |
| Baseline9Work | `38` | Indicates Baseline9 Work task usage view field. |
| Baseline9Cost | `39` | Indicates Baseline9 Cost task usage view field. |
| Baseline10Work | `40` | Indicates Baseline10 Work task usage view field. |
| Baseline10Cost | `41` | Indicates Baseline10 Cost task usage view field. |
| ActualFixedCost | `42` | Indicates Actual Fixed Cost task usage view field. |
| CPI | `43` | Indicates CPI task usage view field. |
| SPI | `44` | Indicates SPI task usage view field. |
| CVPercent | `45` | Indicates CV Percent task usage view field. |
| SVPercent | `46` | Indicates SV Percent task usage view field. |
| BudgetWork | `47` | Indicates Budget Work task usage view field. |
| BudgetCost | `48` | Indicates Budget Cost task usage view field. |
| BaselineBudgetWork | `49` | Indicates Baseline Budget Work task usage view field. |
| BaselineBudgetCost | `50` | Indicates Baseline Budget Cost task usage view field. |
| Baseline1BudgetWork | `51` | Indicates Baseline1 Budget Work task usage view field. |
| Baseline1BudgetCost | `52` | Indicates Baseline1 Budget Cost task usage view field. |
| Baseline2BudgetWork | `53` | Indicates Baseline2 Budget Work task usage view field. |
| Baseline2BudgetCost | `54` | Indicates Baseline2 Budget Cost task usage view field. |
| Baseline3BudgetWork | `55` | Indicates Baseline3 Budget Work task usage view field. |
| Baseline3BudgetCost | `56` | Indicates Baseline3 Budget Cost task usage view field. |
| Baseline4BudgetWork | `57` | Indicates Baseline4 Budget Work task usage view field. |
| Baseline4BudgetCost | `58` | Indicates Baseline4 Budget Cost task usage view field. |
| Baseline5BudgetWork | `59` | Indicates Baseline5 Budget Work task usage view field. |
| Baseline5BudgetCost | `60` | Indicates Baseline5 Budget Cost task usage view field. |
| Baseline6BudgetWork | `61` | Indicates Baseline6 Budget Work task usage view field. |
| Baseline6BudgetCost | `62` | Indicates Baseline6 Budget Cost task usage view field. |
| Baseline7BudgetWork | `63` | Indicates Baseline7 Budget Work task usage view field. |
| Baseline7BudgetCost | `64` | Indicates Baseline7 Budget Cost task usage view field. |
| Baseline8BudgetWork | `65` | Indicates Baseline8 Budget Work task usage view field. |
| Baseline8BudgetCost | `66` | Indicates Baseline8 Budget Cost task usage view field. |
| Baseline9BudgetWork | `67` | Indicates Baseline9 Budget Work task usage view field. |
| Baseline9BudgetCost | `68` | Indicates Baseline9 Budget Cost task usage view field. |
| Baseline10BudgetWork | `69` | Indicates Baseline10 Budget Work task usage view field. |
| Baseline10BudgetCost | `70` | Indicates Baseline10 Budget Cost task usage view field. |
| AllTaskRows | `71` | Indicates All Task Rows task usage view field. |
| AllAssignmentRows | `72` | Indicates All Assignment Rows task usage view field. |

## Examples

Shows how to work field collection of a TaskUsageView instance.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = (TaskUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}

// one can transform collection into a list of TaskUsageViewField
IList<TaskUsageViewField> fields = view.FieldCollection.ToList();
foreach (var field in fields)
{
    Console.WriteLine("Field (from the list): " + field);
}
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


