---
title: Class ExtendedAttributeDefinitionCollection
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.ExtendedAttributeDefinitionCollection class. Represents a collection of ExtendedAttributeDefinition objects
type: docs
weight: 550
url: /net/aspose.tasks/extendedattributedefinitioncollection/
---
## ExtendedAttributeDefinitionCollection class

Represents a collection of [`ExtendedAttributeDefinition`](../extendedattributedefinition/) objects.

```csharp
public class ExtendedAttributeDefinitionCollection : IList<ExtendedAttributeDefinition>
```

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.tasks/extendedattributedefinitioncollection/count/) { get; } | Gets the number of elements contained in this collection. |
| [IsReadOnly](../../aspose.tasks/extendedattributedefinitioncollection/isreadonly/) { get; } | Gets a value indicating whether this collection is read-only. |
| [Item](../../aspose.tasks/extendedattributedefinitioncollection/item/) { get; set; } | Returns or sets the element at the specified index. |
| [ParentProject](../../aspose.tasks/extendedattributedefinitioncollection/parentproject/) { get; } | Gets a parent project for the `ExtendedAttributeDefinitionCollection` instance. returns a parent project for this collection. |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.tasks/extendedattributedefinitioncollection/add/)(ExtendedAttributeDefinition) | Adds the specified item to this collection. |
| [Clear](../../aspose.tasks/extendedattributedefinitioncollection/clear/)() | Removes all items from this collection. |
| [Contains](../../aspose.tasks/extendedattributedefinitioncollection/contains/)(ExtendedAttributeDefinition) | Returns true if the specified item is found in this collection; otherwise, false. |
| [CopyTo](../../aspose.tasks/extendedattributedefinitioncollection/copyto/)(ExtendedAttributeDefinition[], int) | Copies the elements of this collection to the specified array, starting at the specified array index. |
| [GetById](../../aspose.tasks/extendedattributedefinitioncollection/getbyid/)(int) | Returns an extended attribute definition by id |
| [GetEnumerator](../../aspose.tasks/extendedattributedefinitioncollection/getenumerator/)() | Returns an enumerator for this collection. |
| [IndexOf](../../aspose.tasks/extendedattributedefinitioncollection/indexof/)(ExtendedAttributeDefinition) | Determines the index of the specified item in this collection. |
| [Insert](../../aspose.tasks/extendedattributedefinitioncollection/insert/)(int, ExtendedAttributeDefinition) | Inserts the specified item at the specified index. |
| [Remove](../../aspose.tasks/extendedattributedefinitioncollection/remove/)(ExtendedAttributeDefinition) | Removes the first occurrence of a specific object from this collection. |
| [RemoveAt](../../aspose.tasks/extendedattributedefinitioncollection/removeat/)(int) | Removes an item at the specified index. |
| [ToList](../../aspose.tasks/extendedattributedefinitioncollection/tolist/)() | Converts this ExtendedAttributeDefinitionCollection object to a list containing instances of the [`ExtendedAttributeDefinition`](../extendedattributedefinition/) class. |

## Examples

Shows how to use extended attribute definition collections.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

if (!project.ExtendedAttributes.IsReadOnly)
{
    if (project.ExtendedAttributes.Count > 0)
    {
        // clear extended attribute definitions
        project.ExtendedAttributes.Clear();
    }
}

// create extended attribute definition for a task
var taskDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Start, ExtendedAttributeTask.Start7, "Start 7");
project.ExtendedAttributes.Add(taskDefinition);

Console.WriteLine("Iterate over extended attributes of " + project.ExtendedAttributes.ParentProject.Get(Prj.Name) + " project: ");
foreach (var attribute in project.ExtendedAttributes)
{
    Console.WriteLine("Attribute Alias: " + attribute.Alias);
    Console.WriteLine("Attribute CfType: " + attribute.CfType);
    Console.WriteLine();
}

Console.WriteLine();

// work with extended attribute definitions...
var resourceDefinition = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Cost, ExtendedAttributeResource.Cost5, "My cost");

if (!project.ExtendedAttributes.Contains(resourceDefinition))
{
    project.ExtendedAttributes.Add(resourceDefinition);
}

// work with extended attribute definitions...
var resourceDefinition2 = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Number, ExtendedAttributeResource.Cost1, "My Cost 2");

if (project.ExtendedAttributes.IndexOf(resourceDefinition2) < 0)
{
    project.ExtendedAttributes.Insert(0, resourceDefinition2);
}

// work with extended attribute definitions...

// remove extended attribute by index
project.ExtendedAttributes.RemoveAt(0);

Console.WriteLine("Print project's extended attributes: ");
Console.WriteLine("Count of project's extended attribute definitions: " + project.ExtendedAttributes.Count);

// use collection index access
Console.WriteLine("Attribute 1 Alias: " + project.ExtendedAttributes[0].Alias);
Console.WriteLine("Attribute 1 CfType: " + project.ExtendedAttributes[0].CfType);
Console.WriteLine("Attribute 2 Alias: " + project.ExtendedAttributes[1].Alias);
Console.WriteLine("Attribute 2 CfType: " + project.ExtendedAttributes[1].CfType);

var otherProject = new Project();

// copy attributes to other project
var attributes = new ExtendedAttributeDefinition[project.ExtendedAttributes.Count];
project.ExtendedAttributes.CopyTo(attributes, 0);

foreach (var attribute in attributes)
{
    otherProject.ExtendedAttributes.Add(attribute);
}

Console.WriteLine();
Console.WriteLine("Iterate over other project's extended attributes: ");
foreach (var attribute in otherProject.ExtendedAttributes)
{
    Console.WriteLine("Attribute Alias: " + attribute.Alias);
    Console.WriteLine("Attribute CfType: " + attribute.CfType);
    Console.WriteLine();
}

// remove all extended attribute definitions
List<ExtendedAttributeDefinition> definitions = project.ExtendedAttributes.ToList();
foreach (var definition in definitions)
{
    project.ExtendedAttributes.Remove(definition);
}
```

### See Also

* class [ExtendedAttributeDefinition](../extendedattributedefinition/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


