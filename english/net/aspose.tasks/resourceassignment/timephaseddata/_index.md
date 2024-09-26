---
title: ResourceAssignment.TimephasedData
second_title: Aspose.Tasks for .NET API Reference
description: ResourceAssignment property. Gets or sets the instance of TimephasedDataCollection class containing elements of TimephasedData class
type: docs
weight: 600
url: /net/aspose.tasks/resourceassignment/timephaseddata/
---
## ResourceAssignment.TimephasedData property

Gets or sets the instance of [`TimephasedDataCollection`](../../timephaseddatacollection/) class containing elements of `TimephasedData` class.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## Examples

Shows how to read timephased data of a resource assignment.

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");
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
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

// get timephased data
foreach (var td in assn.TimephasedData)
{
    Console.WriteLine(td.Value);
}
```

### See Also

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


