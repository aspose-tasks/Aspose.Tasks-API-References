---
title: Task.SplitParts
second_title: Aspose.Tasks for .NET API Reference
description: Task property. Gets a SplitPart collection that represents the portions of a task
type: docs
weight: 1110
url: /net/aspose.tasks/task/splitparts/
---
## Task.SplitParts property

Gets a SplitPart collection that represents the portions of a task.

```csharp
public SplitPartCollection SplitParts { get; }
```

## Examples

Shows how to display task's split parts.

```csharp
var project = new Project(DataDir + "ViewSplitTasks.mpp");

// Access task 
var task = project.RootTask.Children.GetById(4);

// Display split parts of task
var collection = task.SplitParts;
foreach (var splitPart in collection)
{
    Console.WriteLine("Start: " + splitPart.Start + "\nFinish: " + splitPart.Finish + "\n");
}
```

### See Also

* class [SplitPartCollection](../../splitpartcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


