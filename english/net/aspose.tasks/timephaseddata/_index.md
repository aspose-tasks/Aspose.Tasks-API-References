---
title: Class TimephasedData
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.TimephasedData class. Represents a time phased data
type: docs
weight: 2540
url: /net/aspose.tasks/timephaseddata/
---
## TimephasedData class

Represents a time phased data.

```csharp
public class TimephasedData
```

## Constructors

| Name | Description |
| --- | --- |
| [TimephasedData](timephaseddata/)() | Initializes a new instance of the `TimephasedData` class. |

## Properties

| Name | Description |
| --- | --- |
| [Finish](../../aspose.tasks/timephaseddata/finish/) { get; set; } | Gets or sets the finish date of a time phased data period. |
| [Start](../../aspose.tasks/timephaseddata/start/) { get; set; } | Gets or sets the start date of a time phased data period. |
| [TimephasedDataType](../../aspose.tasks/timephaseddata/timephaseddatatype/) { get; set; } | Gets or sets the type of a time phased data. |
| [Uid](../../aspose.tasks/timephaseddata/uid/) { get; set; } | Gets or sets the unique identifier of a time phased data |
| [Unit](../../aspose.tasks/timephaseddata/unit/) { get; set; } | Gets or sets the time unit of a time phased data period. |
| [Value](../../aspose.tasks/timephaseddata/value/) { get; set; } | Gets or sets the value per unit of time for a time phased data period. |
| [ValueToCost](../../aspose.tasks/timephaseddata/valuetocost/) { get; set; } | Gets Double instance which represents string value of this object. |
| [ValueToDuration](../../aspose.tasks/timephaseddata/valuetoduration/) { get; } | Gets TimeSpan instance which represents string value of this object. |
| [ValueToUnits](../../aspose.tasks/timephaseddata/valuetounits/) { get; } | Gets Double instance which represents string value of this object for unit-based time phased data. |

## Methods

| Name | Description |
| --- | --- |
| static [CreateCostTimephased](../../aspose.tasks/timephaseddata/createcosttimephased/#createcosttimephased)(int, DateTime, DateTime, double, TimephasedDataType) | Creates and initializes a new instance of the `TimephasedData` class for cost-based time phased data. |
| static [CreateCostTimephased](../../aspose.tasks/timephaseddata/createcosttimephased/#createcosttimephased_1)(int, DateTime, DateTime, double, TimeUnitType, TimephasedDataType) | Creates and initializes a new instance of the `TimephasedData` class for cost-based time phased data. |
| static [CreateUnitTimephased](../../aspose.tasks/timephaseddata/createunittimephased/)(int, DateTime, DateTime, double, TimephasedDataType) | Creates and initializes a new instance of the `TimephasedData` class for unit-based time phased data of an assignment of a material resource. |
| static [CreateWorkTimephased](../../aspose.tasks/timephaseddata/createworktimephased/)(int, DateTime, DateTime, TimeSpan, TimeUnitType, TimephasedDataType) | Creates and initializes a new instance of the `TimephasedData` class for work-based time phased data. |

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


