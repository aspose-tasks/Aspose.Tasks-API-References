---
title: SplitPartCollection.Item
second_title: Aspose.Tasks for .NET API Reference
description: SplitPartCollection property. Retrieves a tasks split part at the given index
type: docs
weight: 20
url: /net/aspose.tasks/splitpartcollection/item/
---
## SplitPartCollection indexer

Retrieves a task's split part at the given index.

```csharp
public SplitPart this[int index] { get; set; }
```

| Parameter | Description |
| --- | --- |
| index | The part index. |

### Return Value

a split part.

## Remarks

The index is zero-based. Returns null if the index is outside array's boundaries.

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


