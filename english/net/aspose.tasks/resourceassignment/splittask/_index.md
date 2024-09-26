---
title: ResourceAssignment.SplitTask
second_title: Aspose.Tasks for .NET API Reference
description: ResourceAssignment method. Splits task into two parts
type: docs
weight: 770
url: /net/aspose.tasks/resourceassignment/splittask/
---
## ResourceAssignment.SplitTask method

Splits task into two parts.

```csharp
public void SplitTask(DateTime start, DateTime finish, Calendar calendar)
```

| Parameter | Type | Description |
| --- | --- | --- |
| start | DateTime | The beginning of work interruption to split based on. |
| finish | DateTime | The end of work interruption to split based on. |
| calendar | Calendar | The calendar to split based on. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | Throws when start date is less than the assignment start date. |
| ArgumentOutOfRangeException | Throws when finish date is greater than the assignment finish date. |

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


