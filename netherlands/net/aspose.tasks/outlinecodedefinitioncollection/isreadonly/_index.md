---
title: "OutlineCodeDefinitionCollection.IsReadOnly"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "OutlineCodeDefinitionCollection‑eigenschap. Haalt een waarde op die aangeeft of deze collectie alleen‑lezen is, anders false"
type: docs
weight: 20
url: /nl/net/aspose.tasks/outlinecodedefinitioncollection/isreadonly/
---
## OutlineCodeDefinitionCollection.IsReadOnly property

Haalt een waarde op die aangeeft of deze collectie alleen-lezen is; anders, false.

```csharp
public bool IsReadOnly { get; }
```

## Voorbeelden

Toont hoe te werken met collecties van outline-code-definities.

```csharp
var project = new Project(DataDir + "OutlineCodes.mpp");

Console.WriteLine("Count of outline code definitions: " + project.OutlineCodes.Count);
foreach (var outlineCode in project.OutlineCodes)
{
    Console.WriteLine("Field Name: " + outlineCode.FieldName);
    Console.WriteLine("Alias: " + outlineCode.Alias);
    Console.WriteLine();
}

// voeg een aangepaste outline code-definitie toe
var outlineCodeDefinition = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode3).ToString("D"), Alias = "My Outline Code" };

var outlineCodeDefinition2 = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode1).ToString("D"), Alias = "My Outline Code 2" };

if (!project.OutlineCodes.IsReadOnly)
{
    project.OutlineCodes.Add(outlineCodeDefinition);

    // voeg outline-code-definitie in op positie
    project.OutlineCodes.Insert(0, outlineCodeDefinition2);
}

// zoek de index van de outline-code-definitie
var index = project.OutlineCodes.IndexOf(outlineCodeDefinition);

// bewerk de outline code-definitie
project.OutlineCodes[index].Alias = "New Alias";

// ...
// werken met outline code-definities
// ...

// verwijder de outline code-definitie
if (project.OutlineCodes.Contains(outlineCodeDefinition))
{
    project.OutlineCodes.Remove(outlineCodeDefinition);
}

// verwijder een outline code-definitie op index
project.OutlineCodes.RemoveAt(0);

var otherProject = new Project(DataDir + "Blank2010.mpp");

// verwijder outline code-definities
otherProject.OutlineCodes.Clear();

// kopieer outline code-definities
var outlineCodeDefinitions = new OutlineCodeDefinition[project.OutlineCodes.Count];
project.OutlineCodes.CopyTo(outlineCodeDefinitions, 0);

foreach (var definition in outlineCodeDefinitions)
{
    otherProject.OutlineCodes.Add(definition);
}

// ...
// werken met outline code-definities
// ...

// verwijder outline code-definities één voor één
List<OutlineCodeDefinition> definitions = otherProject.OutlineCodes.ToList();
foreach (var definition in definitions)
{
    otherProject.OutlineCodes.Remove(definition);
}
```

### Zie ook

* class [OutlineCodeDefinitionCollection](../)
* namespace [Aspose.Tasks](../../outlinecodedefinitioncollection/)
* assembly [Aspose.Tasks](../../../)


