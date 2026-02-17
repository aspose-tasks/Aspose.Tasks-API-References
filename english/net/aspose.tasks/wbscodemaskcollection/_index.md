---
title: Class WBSCodeMaskCollection
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.WBSCodeMaskCollection class. Represents a collection of WBSCodeMask objects
type: docs
weight: 3490
url: /net/aspose.tasks/wbscodemaskcollection/
---
## WBSCodeMaskCollection class

Represents a collection of WBSCodeMask objects.

```csharp
public class WBSCodeMaskCollection : IList<WBSCodeMask>
```

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.tasks/wbscodemaskcollection/count/) { get; } | Gets the number of elements contained in this collection. |
| [IsReadOnly](../../aspose.tasks/wbscodemaskcollection/isreadonly/) { get; } | Gets a value indicating whether this collection is read-only; otherwise, false. |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.tasks/wbscodemaskcollection/add/)(WBSCodeMask) | Adds the specified item to this collection. |
| [Clear](../../aspose.tasks/wbscodemaskcollection/clear/)() | Removes all items from this collection. |
| [Contains](../../aspose.tasks/wbscodemaskcollection/contains/)(WBSCodeMask) | Returns true if the specified item is found in this collection; otherwise, false. |
| [CopyTo](../../aspose.tasks/wbscodemaskcollection/copyto/)(WBSCodeMask[], int) | Copies the elements of this collection to the specified array, starting at the specified array index. |
| [GetEnumerator](../../aspose.tasks/wbscodemaskcollection/getenumerator/)() | Returns an enumerator for this collection. |
| [Remove](../../aspose.tasks/wbscodemaskcollection/remove/)(WBSCodeMask) | Removes the first occurrence of a specific object from this collection. |
| [ToList](../../aspose.tasks/wbscodemaskcollection/tolist/)() | Converts a WBSCodeMaskCollection to a list of [`WBSCodeMask`](../wbscodemask/) objects. |

## Examples

Shows how to work with WBS code mask collection.

```csharp
var project = new Project();

project.WBSCodeDefinition = new WBSCodeDefinition();
project.WBSCodeDefinition.GenerateWBSCode = true;
project.WBSCodeDefinition.VerifyUniqueness = true;
project.WBSCodeDefinition.CodePrefix = "CRS-";

project.WBSCodeDefinition.CodeMaskCollection.Clear();

var mask1 = new WBSCodeMask();
mask1.Length = 2;
mask1.Separator = "-";
mask1.Sequence = WBSSequence.OrderedNumbers;
project.WBSCodeDefinition.CodeMaskCollection.Add(mask1);

var mask2 = new WBSCodeMask();
mask2.Length = 1;
mask2.Separator = "-";
mask2.Sequence = WBSSequence.OrderedUppercaseLetters;
project.WBSCodeDefinition.CodeMaskCollection.Add(mask2);

Console.WriteLine("WBS Code mask's count: " + project.WBSCodeDefinition.CodeMaskCollection.Count);
Console.WriteLine("Is WBS Code mask collection read-only?: " + project.WBSCodeDefinition.CodeMaskCollection.IsReadOnly);
Console.WriteLine("Masks: ");
Console.WriteLine();
foreach (var wbsMask in project.WBSCodeDefinition.CodeMaskCollection)
{
    Console.WriteLine("Length: " + wbsMask.Length);
    Console.WriteLine("Level: " + wbsMask.Level);
    Console.WriteLine("Separator: " + wbsMask.Separator);
    Console.WriteLine("Sequence: " + wbsMask.Sequence);
    Console.WriteLine();
}

var task1 = project.RootTask.Children.Add("Task 1");
task1.Children.Add("Task 2");

project.Recalculate();

IEnumerable<Task> childTasks = project.RootTask.SelectAllChildTasks();
foreach (var childTask in childTasks)
{
    Console.WriteLine("Task name: " + childTask.Get(Tsk.Name));
    Console.WriteLine("Task WBS code: " + childTask.Get(Tsk.WBS));
}

project.WBSCodeDefinition.CodeMaskCollection.Remove(mask2);

if (project.WBSCodeDefinition.CodeMaskCollection.Contains(mask2))
{
    throw new InvalidOperationException("WBS code mask wasn't removed.");
}

var otherProject = new Project();
otherProject.WBSCodeDefinition = new WBSCodeDefinition();
otherProject.WBSCodeDefinition.GenerateWBSCode = true;
otherProject.WBSCodeDefinition.VerifyUniqueness = true;
otherProject.WBSCodeDefinition.CodePrefix = "CRS-";

// copy code masks to other project
var masks = new WBSCodeMask[project.WBSCodeDefinition.CodeMaskCollection.Count];
project.WBSCodeDefinition.CodeMaskCollection.CopyTo(masks, 0);

foreach (var mask in masks)
{
    otherProject.WBSCodeDefinition.CodeMaskCollection.Add(mask);
}

List<WBSCodeMask> wbsMasks = otherProject.WBSCodeDefinition.CodeMaskCollection.ToList();
foreach (var wbsMask in wbsMasks)
{
    Console.WriteLine("Length: " + wbsMask.Length);
    Console.WriteLine("Level: " + wbsMask.Level);
    Console.WriteLine("Separator: " + wbsMask.Separator);
    Console.WriteLine("Sequence: " + wbsMask.Sequence);
    Console.WriteLine();
}

var otherTask1 = project.RootTask.Children.Add("Other task 1");
otherTask1.Children.Add("Other task 2");

otherProject.Recalculate();

Console.WriteLine("Print WBS codes of the other project: ");
IEnumerable<Task> otherChildTasks = otherProject.RootTask.SelectAllChildTasks();
foreach (var childTask in otherChildTasks)
{
    Console.WriteLine("Task name: " + childTask.Get(Tsk.Name));
    Console.WriteLine("Task WBS code: " + childTask.Get(Tsk.WBS));
}
```

### See Also

* class [WBSCodeMask](../wbscodemask/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


