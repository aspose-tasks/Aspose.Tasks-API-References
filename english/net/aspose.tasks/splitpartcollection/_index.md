---
title: Class SplitPartCollection
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.SplitPartCollection class. Collection that represents the portions of a task
type: docs
weight: 2280
url: /net/aspose.tasks/splitpartcollection/
---
## SplitPartCollection class

Collection that represents the portions of a task.

```csharp
public class SplitPartCollection : IList<SplitPart>
```

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.tasks/splitpartcollection/count/) { get; } | Gets the number of parts in the collection. |
| [Item](../../aspose.tasks/splitpartcollection/item/) { get; set; } | Retrieves a task's split part at the given index. |

## Methods

| Name | Description |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/splitpartcollection/getenumerator/)() | Returns an enumerator for this collection. |
| [ToArray](../../aspose.tasks/splitpartcollection/toarray/)() | Copies all parts from the collection to a new array. |

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

* class [SplitPart](../splitpart/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


