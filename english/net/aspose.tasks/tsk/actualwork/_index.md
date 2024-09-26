---
title: Tsk.ActualWork
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The amount of work that has already been done by resources assigned to tasks
type: docs
weight: 90
url: /net/aspose.tasks/tsk/actualwork/
---
## Tsk.ActualWork field

The amount of work that has already been done by resources assigned to tasks.

```csharp
public static readonly Key<Duration, TaskKey> ActualWork;
```

## Examples

Shows how to read/write Tsk.ActualWork property.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualWork, project.GetWork(1));

Console.WriteLine("Actual Work: " + task.Get(Tsk.ActualWork));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


