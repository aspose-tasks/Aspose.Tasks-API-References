---
title: TreeAlgorithmBase1.PreAlg
second_title: Aspose.Tasks for .NET API Reference
description: TreeAlgorithmBase method. Called before processing of a node of a tree
type: docs
weight: 30
url: /net/aspose.tasks.util/treealgorithmbase-1/prealg/
---
## TreeAlgorithmBase&lt;T&gt;.PreAlg method

Called before processing of a node of a tree.

```csharp
public virtual void PreAlg(T el, int level)
```

| Parameter | Type | Description |
| --- | --- | --- |
| el | T | Node to process. |
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

* class [TreeAlgorithmBase&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../treealgorithmbase-1/)
* assembly [Aspose.Tasks](../../../)


