---
title: Enum ResourceUsageViewField
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.ResourceUsageViewField enum. Represents possible fields in ResourceUsageView object resource usage view field
type: docs
weight: 1760
url: /net/aspose.tasks/resourceusageviewfield/
---
## ResourceUsageViewField enumeration

Represents possible fields in [`ResourceUsageView`](../resourceusageview/) object resource usage view field.

```csharp
public enum ResourceUsageViewField
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Undefined | `-1` | Indicates Undefined resource usage view field resource usage view field. |
| Work | `0` | Indicates Work resource usage view field. |
| OvertimeWork | `1` | Indicates Overtime Work resource usage view field. |
| ActualWork | `2` | Indicates Actual Work resource usage view field. |
| ActualOvertimeWork | `3` | Indicates Actual Overtime Work resource usage view field. |
| CumulativeWork | `4` | Indicates Cumulative Work resource usage view field. |
| BaselineWork | `5` | Indicates Baseline Work resource usage view field. |
| Overallocation | `6` | Indicates Overallocation resource usage view field. |
| PercentAllocation | `7` | Indicates Percent Allocation resource usage view field. |
| PeakUnits | `8` | Indicates Peak Units resource usage view field. |
| Cost | `9` | Indicates Cost resource usage view field. |
| ActualCost | `10` | Indicates Actual Cost resource usage view field. |
| BaselineCost | `11` | Indicates Baseline Cost resource usage view field. |
| CumulativeCost | `12` | Indicates Cumulative Cost resource usage view field. |
| BCWS | `13` | Indicates BCWS resource usage view field. |
| BCWP | `14` | Indicates BCWP resource usage view field. |
| ACWP | `15` | Indicates ACWP resource usage view field. |
| SV | `16` | Indicates SV resource usage view field. |
| CV | `17` | Indicates CV resource usage view field. |
| RegularWork | `18` | Indicates Regular Work resource usage view field. |
| RemainingAvailability | `19` | Indicates Remaining Availability resource usage view field. |
| UnitAvailability | `20` | Indicates Unit Availability resource usage view field. |
| WorkAvailability | `21` | Indicates Work Availability resource usage view field. |
| Baseline1Work | `22` | Indicates Baseline1 Work resource usage view field. |
| Baseline1Cost | `23` | Indicates Baseline1 Cost resource usage view field. |
| Baseline2Work | `24` | Indicates Baseline2 Work resource usage view field. |
| Baseline2Cost | `25` | Indicates Baseline2 Cost resource usage view field. |
| Baseline3Work | `26` | Indicates Baseline3 Work resource usage view field. |
| Baseline3Cost | `27` | Indicates Baseline3 Cost resource usage view field. |
| Baseline4Work | `28` | Indicates Baseline4 Work resource usage view field. |
| Baseline4Cost | `29` | Indicates Baseline4 Cost resource usage view field. |
| Baseline5Work | `30` | Indicates Baseline5 Work resource usage view field. |
| Baseline5Cost | `31` | Indicates Baseline5 Cost resource usage view field. |
| Baseline6Work | `32` | Indicates Baseline6 Work resource usage view field. |
| Baseline6Cost | `33` | Indicates Baseline6 Cost resource usage view field. |
| Baseline7Work | `34` | Indicates Baseline7 Work resource usage view field. |
| Baseline7Cost | `35` | Indicates Baseline7 Cost resource usage view field. |
| Baseline8Work | `36` | Indicates Baseline8 Work resource usage view field. |
| Baseline8Cost | `37` | Indicates Baseline8 Cost resource usage view field. |
| Baseline9Work | `38` | Indicates Baseline9 Work resource usage view field. |
| Baseline9Cost | `39` | Indicates Baseline9 Cost resource usage view field. |
| Baseline10Work | `40` | Indicates Baseline10 Work resource usage view field. |
| Baseline10Cost | `41` | Indicates Baseline10 Cost resource usage view field. |
| BudgetWork | `42` | Indicates Budget Work resource usage view field. |
| BudgetCost | `43` | Indicates Budget Cost resource usage view field. |
| BaselineBudgetWork | `44` | Indicates Baseline Budget Work resource usage view field. |
| BaselineBudgetCost | `45` | Indicates Baseline Budget Cost resource usage view field. |
| Baseline1BudgetWork | `46` | Indicates Baseline1 Budget Work resource usage view field. |
| Baseline1BudgetCost | `47` | Indicates Baseline1 Budget Cost resource usage view field. |
| Baseline2BudgetWork | `48` | Indicates Baseline2 Budget Work resource usage view field. |
| Baseline2BudgetCost | `49` | Indicates Baseline2 Budget Cost resource usage view field. |
| Baseline3BudgetWork | `50` | Indicates Baseline3 Budget Work resource usage view field. |
| Baseline3BudgetCost | `51` | Indicates Baseline3 Budget Cost resource usage view field. |
| Baseline4BudgetWork | `52` | Indicates Baseline4 Budget Work resource usage view field. |
| Baseline4BudgetCost | `53` | Indicates Baseline4 Budget Cost resource usage view field. |
| Baseline5BudgetWork | `54` | Indicates Baseline5 Budget Work resource usage view field. |
| Baseline5BudgetCost | `55` | Indicates Baseline5 Budget Cost resource usage view field. |
| Baseline6BudgetWork | `56` | Indicates Baseline6 Budget Work resource usage view field. |
| Baseline6BudgetCost | `57` | Indicates Baseline6 Budget Cost resource usage view field. |
| Baseline7BudgetWork | `58` | Indicates Baseline7 Budget Work resource usage view field. |
| Baseline7BudgetCost | `59` | Indicates Baseline7 Budget Cost resource usage view field. |
| Baseline8BudgetWork | `60` | Indicates Baseline8 Budget Work resource usage view field. |
| Baseline8BudgetCost | `61` | Indicates Baseline8 Budget Cost resource usage view field. |
| Baseline9BudgetWork | `62` | Indicates Baseline9 Budget Work resource usage view field. |
| Baseline9BudgetCost | `63` | Indicates Baseline9 Budget Cost resource usage view field. |
| Baseline10BudgetWork | `64` | Indicates Baseline10 Budget Work resource usage view field. |
| Baseline10BudgetCost | `65` | Indicates Baseline10 Budget Cost resource usage view field. |
| AllResourceRows | `66` | Indicates All Resource Rows resource usage view field. |
| AllAssignmentRows | `67` | Indicates All Assignment Rows resource usage view field. |

## Examples

Shows how to read resource usage view fields.

```csharp
var project = new Project(DataDir + "ResourceUsageView.mpp");

var view = (ResourceUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


