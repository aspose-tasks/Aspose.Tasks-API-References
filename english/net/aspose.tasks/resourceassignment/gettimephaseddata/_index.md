---
title: ResourceAssignment.GetTimephasedData
second_title: Aspose.Tasks for .NET API Reference
description: ResourceAssignment method. Returns the instance TimephasedDataCollection class containing instances of TimephasedData class within given start and end dates of specified TimephasedDataType
type: docs
weight: 720
url: /net/aspose.tasks/resourceassignment/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

Returns the instance [`TimephasedDataCollection`](../../timephaseddatacollection/) class containing instances of [`TimephasedData`](../timephaseddata/) class within given start and end dates of specified [`TimephasedDataType`](../../timephaseddatatype/).

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end, 
    TimephasedDataType timephasedType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| start | DateTime | The start date for the time phased data. |
| end | DateTime | The end date for the time phased data. |
| timephasedType | TimephasedDataType | The type of time phased data ([`TimephasedDataType`](../../timephaseddatatype/)). |

### Return Value

returns a list which contains instances of [`TimephasedData`](../../timephaseddata/) class.

## Examples

Shows how to generate timephased data of a resource assignment within a date range.

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");

// Set project properties
project.Set(Prj.StartDate, new DateTime(2013, 10, 30, 9, 0, 0));
project.Set(Prj.NewTasksAreManual, false);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Duration, project.GetDuration(6));

var rsc = project.Resources.Add("Rsc");
rsc.Set(Rsc.StandardRate, 10);
rsc.Set(Rsc.OvertimeRate, 15);

// Create resource assignment
var assn = project.ResourceAssignments.Add(task, rsc);
assn.Set(Asn.Stop, DateTime.MinValue);
assn.Set(Asn.Resume, DateTime.MinValue);

// Set Backloaded contour, it increases task duration from 6 to 10 days
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

project.SetBaseline(BaselineType.Baseline);
task.Set(Tsk.PercentComplete, 50);

// get timephased data
List<TimephasedData> td = assn.GetTimephasedData(assn.Get(Asn.Start), assn.Get(Asn.Finish), TimephasedDataType.AssignmentRemainingWork).ToList();
Console.WriteLine(td.Count);
foreach (var timePhasedValue in td)
{
    Console.WriteLine(timePhasedValue.Value);
}
```

### See Also

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

Returns [`TimephasedDataCollection`](../../timephaseddatacollection/) object with the instances of [`TimephasedData`](../timephaseddata/) class within given start and end dates of AssignmentWork.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| Parameter | Type | Description |
| --- | --- | --- |
| start | DateTime | The start date for the time phased data. |
| end | DateTime | The end date for the time phased data. |

### Return Value

returns a list containing instances of [`TimephasedData`](../../timephaseddata/) class.

## Examples

Shows how to generate timephased data of a resource assignment within a date range.

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");

// Set project properties
project.Set(Prj.StartDate, new DateTime(2013, 10, 30, 9, 0, 0));
project.Set(Prj.NewTasksAreManual, false);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Duration, project.GetDuration(6));

var rsc = project.Resources.Add("Rsc");
rsc.Set(Rsc.StandardRate, 10);
rsc.Set(Rsc.OvertimeRate, 15);

// Create resource assignment
var assn = project.ResourceAssignments.Add(task, rsc);
assn.Set(Asn.Stop, DateTime.MinValue);
assn.Set(Asn.Resume, DateTime.MinValue);

// Set Backloaded contour, it increases task duration from 6 to 10 days
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

project.SetBaseline(BaselineType.Baseline);
task.Set(Tsk.PercentComplete, 50);

// get timephased data
List<TimephasedData> td = assn.GetTimephasedData(assn.Get(Asn.Start), assn.Get(Asn.Finish), TimephasedDataType.AssignmentRemainingWork).ToList();
Console.WriteLine(td.Count);
foreach (var timePhasedValue in td)
{
    Console.WriteLine(timePhasedValue.Value);
}
```

### See Also

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


