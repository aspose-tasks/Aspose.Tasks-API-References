---
title: Tsk.EarlyStart
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The earliest date that a task could possibly begin based on the early start dates of predecessor and successor tasks and other constraints
type: docs
weight: 340
url: /net/aspose.tasks/tsk/earlystart/
---
## Tsk.EarlyStart field

The earliest date that a task could possibly begin, based on the early start dates of predecessor and successor tasks and other constraints.

```csharp
public static readonly Key<DateTime, TaskKey> EarlyStart;
```

## Examples

Shows how to read/write Tsk.EarlyStart property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarlyStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Early Start: " + task.Get(Tsk.EarlyStart));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


