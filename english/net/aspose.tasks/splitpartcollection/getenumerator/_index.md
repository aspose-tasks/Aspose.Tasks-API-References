---
title: SplitPartCollection.GetEnumerator
second_title: Aspose.Tasks for .NET API Reference
description: SplitPartCollection method. Returns an enumerator for this collection
type: docs
weight: 30
url: /net/aspose.tasks/splitpartcollection/getenumerator/
---
## SplitPartCollection.GetEnumerator method

Returns an enumerator for this collection.

```csharp
public IEnumerator<SplitPart> GetEnumerator()
```

### Return Value

an enumerator for this collection.

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


