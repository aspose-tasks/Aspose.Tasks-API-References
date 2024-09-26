---
title: TaskUtils.TaskChildrenCount
second_title: Aspose.Tasks for .NET API Reference
description: TaskUtils method. Recursively calculates a number of tasks children tasks through all levels
type: docs
weight: 40
url: /net/aspose.tasks.util/taskutils/taskchildrencount/
---
## TaskUtils.TaskChildrenCount method

Recursively calculates a number of task's children tasks through all levels.

```csharp
public static int TaskChildrenCount(Task task)
```

| Parameter | Type | Description |
| --- | --- | --- |
| task | Task | The task which children calculate. |

### Return Value

The number of children.

## Examples

Shows how to use &lt;see cref="Aspose.Tasks.Util.TaskUtils.TaskChildrenCount" /&gt; method.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// recursively calculates a number of task's children tasks through all levels
var count = TaskUtils.TaskChildrenCount(project.RootTask);

Console.WriteLine("Number of tasks: " + count);
```

### See Also

* class [Task](../../../aspose.tasks/task/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


