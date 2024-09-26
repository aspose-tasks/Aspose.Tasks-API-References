---
title: Tsk.ActualFinish
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The date when a task was completed
type: docs
weight: 40
url: /net/aspose.tasks/tsk/actualfinish/
---
## Tsk.ActualFinish field

The date when a task was completed.

```csharp
public static readonly Key<DateTime, TaskKey> ActualFinish;
```

## Examples

Shows that project' dates are reset in an evaluation mode.

```csharp
var project = new Project();

// create new tasks
var task1 = project.RootTask.Children.Add("Task1");
task1.Set(Tsk.ActualStart, new DateTime(2000, 2, 10, 8, 0, 0));
task1.Set(Tsk.ActualFinish, new DateTime(2000, 2, 10, 17, 0, 0));

var task2 = project.RootTask.Children.Add("Task2");
task2.Set(Tsk.ActualStart, new DateTime(2000, 2, 10, 8, 0, 0));
task2.Set(Tsk.ActualFinish, new DateTime(2000, 2, 10, 17, 0, 0));

project.Save(OutDir + "EvaluationDateTimeLimitations_out.xml", SaveFileFormat.Xml);
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


