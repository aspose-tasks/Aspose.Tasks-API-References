---
title: "Klasse OutlineCodeDefinitionCollection"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.OutlineCodeDefinitionCollection klasse. Vertegenwoordigt een collectie van OutlineCodeDefinition-objecten."
type: docs
weight: 1180
url: /nl/net/aspose.tasks/outlinecodedefinitioncollection/
---
## OutlineCodeDefinitionCollection class

Vertegenwoordigt een collectie van [`OutlineCodeDefinition`](../outlinecodedefinition/) objecten.

```csharp
public class OutlineCodeDefinitionCollection : IList<OutlineCodeDefinition>
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Count](../../aspose.tasks/outlinecodedefinitioncollection/count/) { get; } | Haalt het aantal elementen op dat in deze collectie zit. |
| [IsReadOnly](../../aspose.tasks/outlinecodedefinitioncollection/isreadonly/) { get; } | Haalt een waarde op die aangeeft of deze collectie alleen-lezen is; anders, false. |
| [Item](../../aspose.tasks/outlinecodedefinitioncollection/item/) { get; set; } | Retourneert of stelt het element in op de opgegeven index. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Add](../../aspose.tasks/outlinecodedefinitioncollection/add/)(OutlineCodeDefinition) | Voegt het opgegeven item toe aan deze collectie. |
| [Clear](../../aspose.tasks/outlinecodedefinitioncollection/clear/)() | Verwijdert alle items uit deze collectie. |
| [Contains](../../aspose.tasks/outlinecodedefinitioncollection/contains/)(OutlineCodeDefinition) | Retourneert true als het opgegeven item in deze collectie wordt gevonden; anders false. |
| [CopyTo](../../aspose.tasks/outlinecodedefinitioncollection/copyto/)(OutlineCodeDefinition[], int) | Kopieert de elementen van deze collectie naar de opgegeven array, beginnend bij de opgegeven array-index. |
| [GetEnumerator](../../aspose.tasks/outlinecodedefinitioncollection/getenumerator/)() | Retourneert een enumerator voor deze collectie. |
| [IndexOf](../../aspose.tasks/outlinecodedefinitioncollection/indexof/)(OutlineCodeDefinition) | Bepaalt de index van het opgegeven item in deze collectie. |
| [Insert](../../aspose.tasks/outlinecodedefinitioncollection/insert/)(int, OutlineCodeDefinition) | Voegt het opgegeven item in op de opgegeven index. |
| [Remove](../../aspose.tasks/outlinecodedefinitioncollection/remove/)(OutlineCodeDefinition) | Verwijdert de eerste instantie van een specifiek object uit deze collectie. |
| [RemoveAt](../../aspose.tasks/outlinecodedefinitioncollection/removeat/)(int) | Verwijdert een item op de opgegeven index. |
| [ToList](../../aspose.tasks/outlinecodedefinitioncollection/tolist/)() | Converteert dit OutlineCodeDefinitionCollection-object naar een lijst van [`OutlineCodeDefinition`](../outlinecodedefinition/) objecten. |

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

* class [OutlineCodeDefinition](../outlinecodedefinition/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


