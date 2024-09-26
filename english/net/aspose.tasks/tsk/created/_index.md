---
title: Tsk.Created
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The date when a task was created
type: docs
weight: 250
url: /net/aspose.tasks/tsk/created/
---
## Tsk.Created field

The date when a task was created.

```csharp
public static readonly Key<DateTime, TaskKey> Created;
```

## Examples

Shows how to read/write Tsk.Created property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Created, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Created: " + task.Get(Tsk.Created));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


