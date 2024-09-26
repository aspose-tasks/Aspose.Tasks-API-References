---
title: Tsk.CommitmentFinish
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The finish date of a delivery.  Reading supported for XML format only
type: docs
weight: 170
url: /net/aspose.tasks/tsk/commitmentfinish/
---
## Tsk.CommitmentFinish field

The finish date of a delivery.  Reading supported for XML format only.

```csharp
public static readonly Key<DateTime, TaskKey> CommitmentFinish;
```

## Examples

Shows how to read/write Tsk.CommitmentFinish property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Commitment Finish: " + task.Get(Tsk.CommitmentFinish));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


