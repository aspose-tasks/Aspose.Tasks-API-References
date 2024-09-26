---
title: CheckCircuit.Alg
second_title: Aspose.Tasks for .NET API Reference
description: CheckCircuit method. Check if the specified object was already processed
type: docs
weight: 20
url: /net/aspose.tasks.util/checkcircuit/alg/
---
## CheckCircuit.Alg method

Check if the specified object was already processed.

```csharp
public override void Alg(Task el, int level)
```

| Parameter | Type | Description |
| --- | --- | --- |
| el | Task | Object to process. |
| level | Int32 | Tree node level. |

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

* class [Task](../../../aspose.tasks/task/)
* class [CheckCircuit](../)
* namespace [Aspose.Tasks.Util](../../checkcircuit/)
* assembly [Aspose.Tasks](../../../)


