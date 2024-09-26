---
title: Tsk.IsActive
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. Determines whether a task is active. Inactive tasks no longer affect other tasks or the overall Project schedule
type: docs
weight: 550
url: /net/aspose.tasks/tsk/isactive/
---
## Tsk.IsActive field

Determines whether a task is active. Inactive tasks no longer affect other tasks or the overall Project schedule.

```csharp
public static readonly Key<NullableBool, TaskKey> IsActive;
```

## Examples

Shows how to read/write Tsk.IsActive property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsActive, true);

Console.WriteLine("Is Active: " + task.Get(Tsk.IsActive));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


