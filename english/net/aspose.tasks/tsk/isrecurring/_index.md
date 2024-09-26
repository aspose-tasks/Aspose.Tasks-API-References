---
title: Tsk.IsRecurring
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. Determines whether a task is part of a series of recurring tasks
type: docs
weight: 670
url: /net/aspose.tasks/tsk/isrecurring/
---
## Tsk.IsRecurring field

Determines whether a task is part of a series of recurring tasks.

```csharp
public static readonly Key<NullableBool, TaskKey> IsRecurring;
```

## Examples

Shows how to read/write Tsk.IsRecurring property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsRecurring, true);

Console.WriteLine("Is Recurring: " + task.Get(Tsk.IsRecurring));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


