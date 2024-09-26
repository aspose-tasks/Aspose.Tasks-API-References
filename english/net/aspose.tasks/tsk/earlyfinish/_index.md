---
title: Tsk.EarlyFinish
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The earliest date that a task could possibly finish based on early finish dates of predecessor and successor tasks other constraints and any leveling delay
type: docs
weight: 330
url: /net/aspose.tasks/tsk/earlyfinish/
---
## Tsk.EarlyFinish field

The earliest date that a task could possibly finish, based on early finish dates of predecessor and successor tasks, other constraints, and any leveling delay.

```csharp
public static readonly Key<DateTime, TaskKey> EarlyFinish;
```

## Examples

Shows how to read/write Tsk.EarlyFinish property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarlyFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Early Finish: " + task.Get(Tsk.EarlyFinish));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


