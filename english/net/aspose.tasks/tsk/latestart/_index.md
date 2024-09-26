---
title: Tsk.LateStart
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The latest date that a task can start without delaying the finish of the project
type: docs
weight: 740
url: /net/aspose.tasks/tsk/latestart/
---
## Tsk.LateStart field

The latest date that a task can start without delaying the finish of the project.

```csharp
public static readonly Key<DateTime, TaskKey> LateStart;
```

## Examples

Shows how to read/write Tsk.LateStart property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LateStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Late Start: " + task.Get(Tsk.LateStart));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


