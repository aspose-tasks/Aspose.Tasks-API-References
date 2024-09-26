---
title: Tsk.PreleveledStart
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The start date of a task as it was before resource leveling was done
type: docs
weight: 920
url: /net/aspose.tasks/tsk/preleveledstart/
---
## Tsk.PreleveledStart field

The start date of a task as it was before resource leveling was done.

```csharp
public static readonly Key<DateTime, TaskKey> PreleveledStart;
```

## Examples

Shows how to read/write Tsk.PreleveledStart property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PreleveledStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Preleveled Start: " + task.Get(Tsk.PreleveledStart));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


