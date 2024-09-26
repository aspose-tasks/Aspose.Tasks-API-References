---
title: Tsk.CommitmentType
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. Determines whether a task has an associated delivery or a dependency on an associated delivery.  Reading supported for XML format only
type: docs
weight: 190
url: /net/aspose.tasks/tsk/commitmenttype/
---
## Tsk.CommitmentType field

Determines whether a task has an associated delivery or a dependency on an associated delivery.  Reading supported for XML format only.

```csharp
public static readonly Key<int, TaskKey> CommitmentType;
```

## Examples

Shows how to read/write Tsk.CommitmentType property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentType, 2);

Console.WriteLine("Commitment Type: " + task.Get(Tsk.CommitmentType));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


