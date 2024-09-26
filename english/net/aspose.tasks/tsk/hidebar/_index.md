---
title: Tsk.HideBar
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. Determines whether the Gantt bar of a task is hidden when displayed in Microsoft Project
type: docs
weight: 480
url: /net/aspose.tasks/tsk/hidebar/
---
## Tsk.HideBar field

Determines whether the Gantt bar of a task is hidden when displayed in Microsoft Project.

```csharp
public static readonly Key<NullableBool, TaskKey> HideBar;
```

## Examples

Shows how to read/write Tsk.HideBar property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.HideBar, true);

Console.WriteLine("Hide Bar: " + task.Get(Tsk.HideBar));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


