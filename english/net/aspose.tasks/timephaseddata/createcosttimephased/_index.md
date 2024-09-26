---
title: TimephasedData.CreateCostTimephased
second_title: Aspose.Tasks for .NET API Reference
description: TimephasedData method. Creates and initializes a new instance of the TimephasedData class for costbased time phased data
type: docs
weight: 20
url: /net/aspose.tasks/timephaseddata/createcosttimephased/
---
## CreateCostTimephased(int, DateTime, DateTime, double, TimeUnitType, TimephasedDataType) {#createcosttimephased_1}

Creates and initializes a new instance of the [`TimephasedData`](../) class for cost-based time phased data.

```csharp
public static TimephasedData CreateCostTimephased(int uid, DateTime start, DateTime finish, 
    double value, TimeUnitType timeUnit, TimephasedDataType type)
```

| Parameter | Type | Description |
| --- | --- | --- |
| uid | Int32 | UID of the task. |
| start | DateTime | start date-time. |
| finish | DateTime | Finish date-time. |
| value | Double | Cost value. |
| timeUnit | TimeUnitType | Time unit type. |
| type | TimephasedDataType | Time-phased data type. |

### Return Value

A instance of the [`TimephasedData`](../) class for cost-based time phased data.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | If negative cost value was specified. |

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

* enum [TimeUnitType](../../timeunittype/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [TimephasedData](../)
* namespace [Aspose.Tasks](../../timephaseddata/)
* assembly [Aspose.Tasks](../../../)

---

## CreateCostTimephased(int, DateTime, DateTime, double, TimephasedDataType) {#createcosttimephased}

Creates and initializes a new instance of the [`TimephasedData`](../) class for cost-based time phased data.

```csharp
public static TimephasedData CreateCostTimephased(int uid, DateTime start, DateTime finish, 
    double value, TimephasedDataType type)
```

| Parameter | Type | Description |
| --- | --- | --- |
| uid | Int32 | UID of the task. |
| start | DateTime | start date-time. |
| finish | DateTime | Finish date-time. |
| value | Double | Cost value. |
| type | TimephasedDataType | Time-phased data type. |

### Return Value

A instance of the [`TimephasedData`](../) class for cost-based time phased data.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | If negative cost value was specified. |

### See Also

* enum [TimephasedDataType](../../timephaseddatatype/)
* class [TimephasedData](../)
* namespace [Aspose.Tasks](../../timephaseddata/)
* assembly [Aspose.Tasks](../../../)


