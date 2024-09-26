---
title: Tsk.PreleveledFinish
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The finish date of a task as it was before resource leveling was done
type: docs
weight: 910
url: /net/aspose.tasks/tsk/preleveledfinish/
---
## Tsk.PreleveledFinish field

The finish date of a task as it was before resource leveling was done.

```csharp
public static readonly Key<DateTime, TaskKey> PreleveledFinish;
```

## Examples

Shows how to read/write Tsk.PreleveledFinish property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PreleveledFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Preleveled Finish: " + task.Get(Tsk.PreleveledFinish));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


