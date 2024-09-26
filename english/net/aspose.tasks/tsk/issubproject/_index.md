---
title: Tsk.IsSubproject
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. Determines whether a task is an inserted project
type: docs
weight: 700
url: /net/aspose.tasks/tsk/issubproject/
---
## Tsk.IsSubproject field

Determines whether a task is an inserted project.

```csharp
public static readonly Key<bool, TaskKey> IsSubproject;
```

## Examples

Shows how to read/write Tsk.IsSubproject property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsSubproject, true);

Console.WriteLine("Is Subproject: " + task.Get(Tsk.IsSubproject));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


