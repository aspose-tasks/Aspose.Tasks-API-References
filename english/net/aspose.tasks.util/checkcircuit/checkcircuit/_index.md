---
title: CheckCircuit.CheckCircuit
second_title: Aspose.Tasks for .NET API Reference
description: CheckCircuit constructor. Initializes a new instance of the CheckCircuit class
type: docs
weight: 10
url: /net/aspose.tasks.util/checkcircuit/checkcircuit/
---
## CheckCircuit constructor

Initializes a new instance of the [`CheckCircuit`](../) class.

```csharp
public CheckCircuit()
```

## Examples

Shows how to detect broken project's structure.

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

// check the project's structure.
// The <see cref="TasksException"> will be thrown if the project structure is incorrect.
try
{
    TaskUtils.Apply(project.RootTask, new CheckCircuit(), 0);
}
catch (TasksException ex)
{
    Console.WriteLine(ex);
}
```

### See Also

* class [CheckCircuit](../)
* namespace [Aspose.Tasks.Util](../../checkcircuit/)
* assembly [Aspose.Tasks](../../../)


