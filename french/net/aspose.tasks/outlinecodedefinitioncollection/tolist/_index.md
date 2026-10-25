---
title: "OutlineCodeDefinitionCollection.ToList"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "OutlineCodeDefinitionCollection méthode. Convertit cet objet OutlineCodeDefinitionCollection en une liste d'objets OutlineCodeDefinition"
type: docs
weight: 130
url: /fr/net/aspose.tasks/outlinecodedefinitioncollection/tolist/
---
## OutlineCodeDefinitionCollection.ToList method

Convertit cet objet OutlineCodeDefinitionCollection en une liste d'objets [`OutlineCodeDefinition`](../../outlinecodedefinition/).

```csharp
public List<OutlineCodeDefinition> ToList()
```

### Valeur de retour

Liste d'objets [`OutlineCodeDefinition`](../../outlinecodedefinition/).

## Exemples

Montre comment travailler avec des collections de outline code definition.

```csharp
var project = new Project(DataDir + "OutlineCodes.mpp");

Console.WriteLine("Count of outline code definitions: " + project.OutlineCodes.Count);
foreach (var outlineCode in project.OutlineCodes)
{
    Console.WriteLine("Field Name: " + outlineCode.FieldName);
    Console.WriteLine("Alias: " + outlineCode.Alias);
    Console.WriteLine();
}

// ajouter une définition de outline code personnalisée
var outlineCodeDefinition = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode3).ToString("D"), Alias = "My Outline Code" };

var outlineCodeDefinition2 = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode1).ToString("D"), Alias = "My Outline Code 2" };

if (!project.OutlineCodes.IsReadOnly)
{
    project.OutlineCodes.Add(outlineCodeDefinition);

    // insérer outline code definition à la position
    project.OutlineCodes.Insert(0, outlineCodeDefinition2);
}

// trouver l'index de l'outline code definition
var index = project.OutlineCodes.IndexOf(outlineCodeDefinition);

// modifier la définition du code de plan
project.OutlineCodes[index].Alias = "New Alias";

// ...
// travailler avec les définitions de code de plan
// ...

// supprimer la définition du code de plan
if (project.OutlineCodes.Contains(outlineCodeDefinition))
{
    project.OutlineCodes.Remove(outlineCodeDefinition);
}

// supprimer une définition de code de plan par indice
project.OutlineCodes.RemoveAt(0);

var otherProject = new Project(DataDir + "Blank2010.mpp");

// supprimer les définitions de code de plan
otherProject.OutlineCodes.Clear();

// copier les définitions de code de plan
var outlineCodeDefinitions = new OutlineCodeDefinition[project.OutlineCodes.Count];
project.OutlineCodes.CopyTo(outlineCodeDefinitions, 0);

foreach (var definition in outlineCodeDefinitions)
{
    otherProject.OutlineCodes.Add(definition);
}

// ...
// travailler avec les définitions de code de plan
// ...

// supprimer les définitions de code de plan une par une
List<OutlineCodeDefinition> definitions = otherProject.OutlineCodes.ToList();
foreach (var definition in definitions)
{
    otherProject.OutlineCodes.Remove(definition);
}
```

### Voir aussi

* class [OutlineCodeDefinition](../../outlinecodedefinition/)
* class [OutlineCodeDefinitionCollection](../)
* namespace [Aspose.Tasks](../../outlinecodedefinitioncollection/)
* assembly [Aspose.Tasks](../../../)


