---
title: Class CheckCircuit
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Util.CheckCircuit class. Checks a tree of tasks whether it contains a circuit
type: docs
weight: 2630
url: /net/aspose.tasks.util/checkcircuit/
---
## CheckCircuit class

Checks a tree (of tasks) whether it contains a circuit.

```csharp
public class CheckCircuit : TreeAlgorithmBase<Task>
```

## Constructors

| Name | Description |
| --- | --- |
| [CheckCircuit](checkcircuit/)() | Initializes a new instance of the `CheckCircuit` class. |

## Methods

| Name | Description |
| --- | --- |
| override [Alg](../../aspose.tasks.util/checkcircuit/alg/)(Task, int) | Check if the specified object was already processed. |
| virtual [PostAlg](../../aspose.tasks.util/treealgorithmbase-1/postalg/)(Task, int) |  |
| virtual [PreAlg](../../aspose.tasks.util/treealgorithmbase-1/prealg/)(Task, int) |  |

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

* class [TreeAlgorithmBase&lt;T&gt;](../treealgorithmbase-1/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


