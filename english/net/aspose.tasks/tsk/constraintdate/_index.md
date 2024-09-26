---
title: Tsk.ConstraintDate
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The specific date associated with the constraint type
type: docs
weight: 200
url: /net/aspose.tasks/tsk/constraintdate/
---
## Tsk.ConstraintDate field

The specific date associated with the constraint type.

```csharp
public static readonly Key<DateTime, TaskKey> ConstraintDate;
```

## Examples

Shows how to get/set a constraint for a task.

```csharp
var project = new Project(DataDir + "ConstraintAsLateAsPossible.mpp");

// Set constraint As Late As Possible for task with Id 11
var newTask = project.RootTask.Children.GetById(11);
newTask.Set(Tsk.ConstraintType, ConstraintType.AsLateAsPossible);

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Parse through all the collected tasks
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.ConstraintType).ToString());
    Console.WriteLine(task.Get(Tsk.ConstraintDate).ToShortDateString() == "1/1/2000" ? "NA" : task.Get(Tsk.ConstraintDate).ToShortDateString());
}

SaveOptions options = new PdfSaveOptions
{
    StartDate = project.Get(Prj.StartDate),
    Timescale = Timescale.ThirdsOfMonths
};

project.Save(OutDir + "SetConstraintAsLateAsPossible_out.pdf", options);
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


