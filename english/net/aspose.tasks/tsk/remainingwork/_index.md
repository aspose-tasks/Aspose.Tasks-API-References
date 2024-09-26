---
title: Tsk.RemainingWork
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The time still required to complete a task or set of tasks
type: docs
weight: 990
url: /net/aspose.tasks/tsk/remainingwork/
---
## Tsk.RemainingWork field

The time still required to complete a task or set of tasks.

```csharp
public static readonly Key<Duration, TaskKey> RemainingWork;
```

## Examples

Shows how to read/write Tsk.RemainingWork property.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingWork, project.GetWork(1));

Console.WriteLine("Remaining Work: " + task.Get(Tsk.RemainingWork));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


