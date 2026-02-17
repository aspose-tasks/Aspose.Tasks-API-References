---
title: Class OutlineCodeDefinitionCollection
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.OutlineCodeDefinitionCollection class. Represents a collection of OutlineCodeDefinition objects
type: docs
weight: 1170
url: /net/aspose.tasks/outlinecodedefinitioncollection/
---
## OutlineCodeDefinitionCollection class

Represents a collection of [`OutlineCodeDefinition`](../outlinecodedefinition/) objects.

```csharp
public class OutlineCodeDefinitionCollection : IList<OutlineCodeDefinition>
```

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.tasks/outlinecodedefinitioncollection/count/) { get; } | Gets the number of elements contained in this collection. |
| [IsReadOnly](../../aspose.tasks/outlinecodedefinitioncollection/isreadonly/) { get; } | Gets a value indicating whether this collection is read-only; otherwise, false. |
| [Item](../../aspose.tasks/outlinecodedefinitioncollection/item/) { get; set; } | Returns or sets the element at the specified index. |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.tasks/outlinecodedefinitioncollection/add/)(OutlineCodeDefinition) | Adds the specified item to this collection. |
| [Clear](../../aspose.tasks/outlinecodedefinitioncollection/clear/)() | Removes all items from this collection. |
| [Contains](../../aspose.tasks/outlinecodedefinitioncollection/contains/)(OutlineCodeDefinition) | Returns true if the specified item is found in this collection; otherwise, false. |
| [CopyTo](../../aspose.tasks/outlinecodedefinitioncollection/copyto/)(OutlineCodeDefinition[], int) | Copies the elements of this collection to the specified array, starting at the specified array index. |
| [GetEnumerator](../../aspose.tasks/outlinecodedefinitioncollection/getenumerator/)() | Returns an enumerator for this collection. |
| [IndexOf](../../aspose.tasks/outlinecodedefinitioncollection/indexof/)(OutlineCodeDefinition) | Determines the index of the specified item in this collection. |
| [Insert](../../aspose.tasks/outlinecodedefinitioncollection/insert/)(int, OutlineCodeDefinition) | Inserts the specified item at the specified index. |
| [Remove](../../aspose.tasks/outlinecodedefinitioncollection/remove/)(OutlineCodeDefinition) | Removes the first occurrence of a specific object from this collection. |
| [RemoveAt](../../aspose.tasks/outlinecodedefinitioncollection/removeat/)(int) | Removes an item at the specified index. |
| [ToList](../../aspose.tasks/outlinecodedefinitioncollection/tolist/)() | Converts this OutlineCodeDefinitionCollection object to a list of [`OutlineCodeDefinition`](../outlinecodedefinition/) objects. |

## Examples

Shows how to work with outline code definition collections.

```csharp
var project = new Project(DataDir + "OutlineCodes.mpp");

Console.WriteLine("Count of outline code definitions: " + project.OutlineCodes.Count);
foreach (var outlineCode in project.OutlineCodes)
{
    Console.WriteLine("Field Name: " + outlineCode.FieldName);
    Console.WriteLine("Alias: " + outlineCode.Alias);
    Console.WriteLine();
}

// add a custom outline code definition
var outlineCodeDefinition = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode3).ToString("D"), Alias = "My Outline Code" };

var outlineCodeDefinition2 = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode1).ToString("D"), Alias = "My Outline Code 2" };

if (!project.OutlineCodes.IsReadOnly)
{
    project.OutlineCodes.Add(outlineCodeDefinition);

    // insert outline code definition in position
    project.OutlineCodes.Insert(0, outlineCodeDefinition2);
}

// find the index of the outline code definition
var index = project.OutlineCodes.IndexOf(outlineCodeDefinition);

// edit the outline code definition
project.OutlineCodes[index].Alias = "New Alias";

// ...
// work with outline code definitions
// ...

// remove the outline code definition
if (project.OutlineCodes.Contains(outlineCodeDefinition))
{
    project.OutlineCodes.Remove(outlineCodeDefinition);
}

// remove an outline code definition by index
project.OutlineCodes.RemoveAt(0);

var otherProject = new Project(DataDir + "Blank2010.mpp");

// remove outline code definitions
otherProject.OutlineCodes.Clear();

// copy outline code definitions
var outlineCodeDefinitions = new OutlineCodeDefinition[project.OutlineCodes.Count];
project.OutlineCodes.CopyTo(outlineCodeDefinitions, 0);

foreach (var definition in outlineCodeDefinitions)
{
    otherProject.OutlineCodes.Add(definition);
}

// ...
// work with outline code definitions
// ...

// remove outline code definitions one by one
List<OutlineCodeDefinition> definitions = otherProject.OutlineCodes.ToList();
foreach (var definition in definitions)
{
    otherProject.OutlineCodes.Remove(definition);
}
```

### See Also

* class [OutlineCodeDefinition](../outlinecodedefinition/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


