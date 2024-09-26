---
title: SplitPartCollection.Count
second_title: Aspose.Tasks for .NET API Reference
description: SplitPartCollection property. Gets the number of parts in the collection
type: docs
weight: 10
url: /net/aspose.tasks/splitpartcollection/count/
---
## SplitPartCollection.Count property

Gets the number of parts in the collection.

```csharp
public int Count { get; }
```

## Examples

Shows how to work with split part collections.

```csharp
var project = new Project(DataDir + "Splits.mpp");

var task = project.RootTask.Children.GetById(1);

// iterate over split parts
Console.WriteLine("Iterate over split parts");
Console.WriteLine("Split parts count:" + task.SplitParts.Count);
foreach (var splitPart in task.SplitParts)
{
    Console.WriteLine("Start: " + splitPart.Start);
    Console.WriteLine("Finish: " + splitPart.Finish);
}

// get the part by index
var split = task.SplitParts[0];
Console.WriteLine("Split start: " + split.Start);

// make some work with the first split part of the task
```

### See Also

* class [SplitPartCollection](../)
* namespace [Aspose.Tasks](../../splitpartcollection/)
* assembly [Aspose.Tasks](../../../)


