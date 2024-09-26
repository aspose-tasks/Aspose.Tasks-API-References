---
title: Tsk.LateFinish
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The latest date that a task can finish without delaying the finish of the project
type: docs
weight: 730
url: /net/aspose.tasks/tsk/latefinish/
---
## Tsk.LateFinish field

The latest date that a task can finish without delaying the finish of the project.

```csharp
public static readonly Key<DateTime, TaskKey> LateFinish;
```

## Examples

Shows how to read/write Tsk.LateFinish property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LateFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Late Finish: " + task.Get(Tsk.LateFinish));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


