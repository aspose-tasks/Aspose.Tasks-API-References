---
title: OutlineCodeDefinitionCollection.RemoveAt
second_title: Aspose.Tasks for .NET API Reference
description: OutlineCodeDefinitionCollection method. Removes an item at the specified index
type: docs
weight: 120
url: /net/aspose.tasks/outlinecodedefinitioncollection/removeat/
---
## OutlineCodeDefinitionCollection.RemoveAt method

Removes an item at the specified index.

```csharp
public void RemoveAt(int index)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | the specified zero-based index to remove an item at. |

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

* class [OutlineCodeDefinitionCollection](../)
* namespace [Aspose.Tasks](../../outlinecodedefinitioncollection/)
* assembly [Aspose.Tasks](../../../)


