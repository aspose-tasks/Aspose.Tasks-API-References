---
title: Tsk.Work
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The total time scheduled on a task for all assigned resources
type: docs
weight: 1150
url: /net/aspose.tasks/tsk/work/
---
## Tsk.Work field

The total time scheduled on a task for all assigned resources.

```csharp
public static readonly Key<Duration, TaskKey> Work;
```

## Examples

Shows how to read/write Tsk.Work property.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Work, project.GetWork(1));

Console.WriteLine("Work: " + task.Get(Tsk.Work));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


