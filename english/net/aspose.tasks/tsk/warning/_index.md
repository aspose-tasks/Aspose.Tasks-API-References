---
title: Tsk.Warning
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. Represents the flag which indicates that task has schedule discrepancies
type: docs
weight: 1120
url: /net/aspose.tasks/tsk/warning/
---
## Tsk.Warning field

Represents the flag which indicates that task has schedule discrepancies.

```csharp
public static readonly Key<bool, TaskKey> Warning;
```

## Examples

Shows how to read a task warning.

```csharp
var project = new Project(DataDir + "schedule-conflict.mpp");
var task = project.RootTask.Children.GetById(1);
Console.WriteLine(task.Get(Tsk.Warning));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


