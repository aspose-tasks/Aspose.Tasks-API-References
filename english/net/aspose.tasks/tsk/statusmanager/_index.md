---
title: Tsk.StatusManager
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The name of the enterprise resource who is to receive status updates for the current task from resources
type: docs
weight: 1050
url: /net/aspose.tasks/tsk/statusmanager/
---
## Tsk.StatusManager field

The name of the enterprise resource who is to receive status updates for the current task from resources.

```csharp
public static readonly Key<string, TaskKey> StatusManager;
```

## Examples

Shows how to read/write Tsk.StatusManager property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StatusManager, "John Smith");

Console.WriteLine("Status Manager: " + task.Get(Tsk.StatusManager));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


