---
title: Tsk.CommitmentStart
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The start date of a delivery. Reading supported for XML format only
type: docs
weight: 180
url: /net/aspose.tasks/tsk/commitmentstart/
---
## Tsk.CommitmentStart field

The start date of a delivery. Reading supported for XML format only.

```csharp
public static readonly Key<DateTime, TaskKey> CommitmentStart;
```

## Examples

Shows how to read/write Tsk.CommitmentStart property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Commitment Start: " + task.Get(Tsk.CommitmentStart));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


