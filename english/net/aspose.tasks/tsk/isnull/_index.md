---
title: Tsk.IsNull
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. Determines whether a task is a null task
type: docs
weight: 640
url: /net/aspose.tasks/tsk/isnull/
---
## Tsk.IsNull field

Determines whether a task is a null task.

```csharp
public static readonly Key<NullableBool, TaskKey> IsNull;
```

## Examples

Shows how to read/write Tsk.IsNull property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsNull, true);

Console.WriteLine("Is Null: " + task.Get(Tsk.IsNull));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


