---
title: SplitPartCollection.ToArray
second_title: Aspose.Tasks for .NET API Reference
description: SplitPartCollection method. Copies all parts from the collection to a new array
type: docs
weight: 40
url: /net/aspose.tasks/splitpartcollection/toarray/
---
## SplitPartCollection.ToArray method

Copies all parts from the collection to a new array.

```csharp
public SplitPart[] ToArray()
```

### Return Value

An array of [`SplitPart`](../../splitpart/) objects.

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

* class [SplitPart](../../splitpart/)
* class [SplitPartCollection](../)
* namespace [Aspose.Tasks](../../splitpartcollection/)
* assembly [Aspose.Tasks](../../../)


