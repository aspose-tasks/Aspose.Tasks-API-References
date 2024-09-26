---
title: ResourceAssignment.TimephasedDataFromTaskDuration
second_title: Aspose.Tasks for .NET API Reference
description: ResourceAssignment method. Generates list of time phased data based on the task duration and the scheduled start date
type: docs
weight: 780
url: /net/aspose.tasks/resourceassignment/timephaseddatafromtaskduration/
---
## ResourceAssignment.TimephasedDataFromTaskDuration method

Generates list of time phased data based on the task duration and the scheduled start date.

```csharp
public void TimephasedDataFromTaskDuration(Calendar calendar)
```

| Parameter | Type | Description |
| --- | --- | --- |
| calendar | Calendar | The calendar to generate time phased data from. |

## Examples

Shows how to add a split for a task.

```csharp
var project = new Project();

// Get a standard calendar
var calendar = project.Get(Prj.Calendar);

// Set project's calendar settings
project.Set(Prj.StartDate, new DateTime(2000, 3, 15, 8, 0, 0));
project.Set(Prj.FinishDate, new DateTime(2000, 4, 21, 17, 0, 0));

// Add a new task to root task
var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Duration, project.GetDuration(3));

// Create a new resource assignment and generate timephased data
var assignment = project.ResourceAssignments.Add(task, null);
assignment.TimephasedDataFromTaskDuration(calendar);

// Split the task into 3 parts.
// Provide start date and finish date arguments to SplitTask method which will be used for split
assignment.SplitTask(new DateTime(2000, 3, 16, 8, 0, 0), new DateTime(2000, 3, 16, 17, 0, 0), calendar);
assignment.SplitTask(new DateTime(2000, 3, 18, 8, 0, 0), new DateTime(2000, 3, 18, 17, 0, 0), calendar);
assignment.Set(Asn.WorkContour, WorkContourType.Contoured);

project.Save(OutDir + "CreateSplitTasks_out.xml", SaveFileFormat.Xml);
```

### See Also

* class [Calendar](../../calendar/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


