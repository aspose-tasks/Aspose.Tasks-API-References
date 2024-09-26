---
title: Tsk.Resume
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The date that the remaining part of a task is scheduled to resume after entering any progress
type: docs
weight: 1000
url: /net/aspose.tasks/tsk/resume/
---
## Tsk.Resume field

The date that the remaining part of a task is scheduled to resume after entering any progress.

```csharp
public static readonly Key<DateTime, TaskKey> Resume;
```

## Examples

Shows how to read task's Stop/Resume dates.

```csharp
var project = new Project(DataDir + "StopResumeDates.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Check Stop and Resume dates for all tasks
foreach (var task in collector.Tasks)
{
    if (task.Get(Tsk.Stop).ToShortDateString() == "1/1/2000")
    {
        Console.WriteLine("Stop: NA");
    }
    else
    {
        Console.WriteLine("Stop: " + task.Get(Tsk.Stop).ToShortDateString());
    }

    if (task.Get(Tsk.Resume).ToShortDateString() == "1/1/2000")
    {
        Console.WriteLine("Resume: NA");
    }
    else
    {
        Console.WriteLine("Resume: " + task.Get(Tsk.Resume).ToShortDateString());
    }
}
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


