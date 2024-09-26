---
title: Tsk.IsPublished
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. Determines whether the current task should be published to Project Server with the rest of the project
type: docs
weight: 660
url: /net/aspose.tasks/tsk/ispublished/
---
## Tsk.IsPublished field

Determines whether the current task should be published to Project Server with the rest of the project.

```csharp
public static readonly Key<NullableBool, TaskKey> IsPublished;
```

## Examples

Shows how to read/write Tsk.IsPublished property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsPublished, true);

Console.WriteLine("Is Published: " + task.Get(Tsk.IsPublished));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


