---
title: Tsk.Guid
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The generated unique identification codes for a task
type: docs
weight: 460
url: /net/aspose.tasks/tsk/guid/
---
## Tsk.Guid field

The generated unique identification codes for a task.

```csharp
public static readonly Key<string, TaskKey> Guid;
```

## Examples

Shows how to read/write Tsk.Guid property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Guid, "60648d59-9c2b-4dc6-bfdb-bfd38f331d61");

Console.WriteLine("Guid: " + task.Get(Tsk.Guid));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


