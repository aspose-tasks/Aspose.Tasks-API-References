---
title: Enum TimephasedDataType
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.TimephasedDataType enum. Specifies the type of time phased data
type: docs
weight: 2560
url: /net/aspose.tasks/timephaseddatatype/
---
## TimephasedDataType enumeration

Specifies the type of time phased data.

```csharp
public enum TimephasedDataType : sbyte
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Undefined | `-1` | Undefined value. |
| AssignmentRemainingWork | `1` | Assignment Remaining Work. |
| AssignmentActualWork | `2` | Assignment Actual Work. |
| AssignmentActualOvertimeWork | `3` | Assignment Actual Overtime Work. |
| AssignmentBaselineWork | `4` | Assignment Baseline Work. |
| AssignmentBaselineCost | `5` | Assignment Baseline Cost. |
| AssignmentActualCost | `6` | Assignment Actual Cost. |
| ResourceBaselineWork | `7` | Resource Baseline Work. |
| ResourceBaselineCost | `8` | Resource Baseline Cost. |
| TaskBaselineWork | `9` | Task Baseline Work. |
| TaskBaselineCost | `10` | Task Baseline Cost. |
| TaskPercentComplete | `11` | Task Percent Complete. |
| AssignmentBaseline1Work | `16` | Assignment Baseline 1 Work |
| AssignmentBaseline1Cost | `17` | Assignment Baseline 1 Cost. |
| TaskBaseline1Work | `18` | Task Baseline 1 Work. |
| TaskBaseline1Cost | `19` | Task Baseline 1 Cost. |
| ResourceBaseline1Work | `20` | Resource Baseline 1 Work. |
| ResourceBaseline1Cost | `21` | Resource Baseline 1 Cost. |
| AssignmentBaseline2Work | `22` | Assignment Baseline 2 Work. |
| AssignmentBaseline2Cost | `23` | Assignment Baseline 2 Cost. |
| TaskBaseline2Work | `24` | Task Baseline 2 Work. |
| TaskBaseline2Cost | `25` | Task Baseline 2 Cost. |
| ResourceBaseline2Work | `26` | Resource Baseline 2 Work. |
| ResourceBaseline2Cost | `27` | Resource Baseline 2 Cost. |
| AssignmentBaseline3Work | `28` | Assignment Baseline 3 Work. |
| AssignmentBaseline3Cost | `29` | Assignment Baseline 3 Cost. |
| TaskBaseline3Work | `30` | Task Baseline 3 Work. |
| TaskBaseline3Cost | `31` | Task Baseline 3 Cost. |
| ResourceBaseline3Work | `32` | Resource Baseline 3 Work. |
| ResourceBaseline3Cost | `33` | Resource Baseline 3 Cost. |
| AssignmentBaseline4Work | `34` | Assignment Baseline 4 Work. |
| AssignmentBaseline4Cost | `35` | Assignment Baseline 4 Cost. |
| TaskBaseline4Work | `36` | Task Baseline 4 Work. |
| TaskBaseline4Cost | `37` | Task Baseline 4 Cost. |
| ResourceBaseline4Work | `38` | Resource Baseline 4 Work. |
| ResourceBaseline4Cost | `39` | Resource Baseline 4 Cost. |
| AssignmentBaseline5Work | `40` | Assignment Baseline 5 Work. |
| AssignmentBaseline5Cost | `41` | Assignment Baseline 5 Cost. |
| TaskBaseline5Work | `42` | Task Baseline 5 Work. |
| TaskBaseline5Cost | `43` | Task Baseline 5 Cost. |
| ResourceBaseline5Work | `44` | Resource Baseline 5 Work. |
| ResourceBaseline5Cost | `45` | Resource Baseline 5 Cost. |
| AssignmentBaseline6Work | `46` | Assignment Baseline 6 Work. |
| AssignmentBaseline6Cost | `47` | Assignment Baseline 6 Cost. |
| TaskBaseline6Work | `48` | Task Baseline 6 Work. |
| TaskBaseline6Cost | `49` | Task Baseline 6 Cost. |
| ResourceBaseline6Work | `50` | Resource Baseline 6 Work. |
| ResourceBaseline6Cost | `51` | Resource Baseline 6 Cost. |
| AssignmentBaseline7Work | `52` | Assignment Baseline 7 Work. |
| AssignmentBaseline7Cost | `53` | Assignment Baseline 7 Cost. |
| TaskBaseline7Work | `54` | Task Baseline 7 Work. |
| TaskBaseline7Cost | `55` | Task Baseline 7 Cost. |
| ResourceBaseline7Work | `56` | Resource Baseline 7 Work |
| ResourceBaseline7Cost | `57` | Resource Baseline 7 Cost. |
| AssignmentBaseline8Work | `58` | Assignment Baseline 8 Work. |
| AssignmentBaseline8Cost | `59` | Assignment Baseline 8 Cost. |
| TaskBaseline8Work | `60` | Task Baseline 8 Work. |
| TaskBaseline8Cost | `61` | Task Baseline 8 Cost. |
| ResourceBaseline8Work | `62` | Resource Baseline 8 Work. |
| ResourceBaseline8Cost | `63` | Resource Baseline 8 Cost. |
| AssignmentBaseline9Work | `64` | Assignment Baseline 9 Work. |
| AssignmentBaseline9Cost | `65` | Assignment Baseline 9 Cost. |
| TaskBaseline9Work | `66` | Task Baseline 9 Work. |
| TaskBaseline9Cost | `67` | Task Baseline 9 Cost. |
| ResourceBaseline9Work | `68` | Resource Baseline 9 Work. |
| ResourceBaseline9Cost | `69` | Resource Baseline 9 Cost. |
| AssignmentBaseline10Work | `70` | Assignment Baseline 10 Work. |
| AssignmentBaseline10Cost | `71` | Assignment Baseline 10 Cost. |
| TaskBaseline10Work | `72` | Task Baseline 10 Work. |
| TaskBaseline10Cost | `73` | Task Baseline 10 Cost. |
| ResourceBaseline10Work | `74` | Resource Baseline 10 Work. |
| ResourceBaseline10Cost | `75` | Resource Baseline 10 Cost. |
| PhysicalPercentComplete | `76` | Physical Percent Complete. |
| TaskWork | `77` | Task Work. |
| TaskCost | `78` | Task Cost. |
| ResourceWork | `79` | Resource Work. |
| ResourceCost | `80` | Resource Cost. |
| AssignmentWork | `81` | Assignment Work. |
| AssignmentCost | `82` | Assignment Cost. |

## Examples

Shows how to work with custom timephased data.

```csharp
var project = new Project(DataDir + "Project1.mpp") { CalculationMode = CalculationMode.None };

var workResource = project.Resources.Add("Work Resource");
workResource.Set(Rsc.Type, ResourceType.Work);
var costResource = project.Resources.Add("Cost Resource");
costResource.Set(Rsc.Type, ResourceType.Cost);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2018, 1, 1, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

var workAssignment = project.ResourceAssignments.Add(task, workResource);
workAssignment.Set(Asn.WorkContour, WorkContourType.Contoured);
var costAssignment = project.ResourceAssignments.Add(task, costResource);
costAssignment.Set(Asn.WorkContour, WorkContourType.Contoured);

// lets add custom timephased tds
workAssignment.TimephasedData.Clear();

// add work days
var td1 = TimephasedData.CreateWorkTimephased(
    workAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 2, 8, 0, 0),
    new DateTime(2018, 1, 5, 17, 0, 0),
    TimeSpan.FromHours(40),
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentRemainingWork);

// add weekend
var td2 = TimephasedData.CreateWorkTimephased(
    workAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 6, 8, 0, 0),
    new DateTime(2018, 1, 8, 8, 0, 0),
    TimeSpan.Zero,
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentRemainingWork);

workAssignment.TimephasedData.Add(td1);
workAssignment.TimephasedData.Add(td2);

costAssignment.TimephasedData.Clear();

// add work days
var td11 = TimephasedData.CreateCostTimephased(
    costAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 2, 8, 0, 0),
    new DateTime(2018, 1, 5, 17, 0, 0),
    1,
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentCost);

// add weekend
var td22 = TimephasedData.CreateCostTimephased(
    costAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 6, 8, 0, 0),
    new DateTime(2018, 1, 8, 8, 0, 0),
    0,
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentCost);

costAssignment.TimephasedData.Add(td11);
costAssignment.TimephasedData.Add(td22);

Console.WriteLine("Print assignment timephased data:");
foreach (var assignment in project.ResourceAssignments)
{
    Console.WriteLine("Assignment UID: " + assignment.Get(Asn.Uid));
    foreach (var tds in assignment.TimephasedData)
    {
        Console.WriteLine("  Uid: " + tds.Uid);
        Console.WriteLine("  Start: " + tds.Start);
        Console.WriteLine("  Finish: " + tds.Finish);
        Console.WriteLine("  Type: " + tds.TimephasedDataType);
        Console.WriteLine("  Unit: " + tds.Unit);
        Console.WriteLine("  Value: " + tds.Value);
        Console.WriteLine("  ValueToCost: " + tds.ValueToCost);
        Console.WriteLine("  ValueToDuration: " + tds.ValueToDuration);
        Console.WriteLine("  ValueToUnits: " + tds.ValueToUnits);
        Console.WriteLine();
    }
}

project.Recalculate();
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


