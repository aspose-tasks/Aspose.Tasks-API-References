---
title: "Classe OutlineCodeDefinitionCollection"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.OutlineCodeDefinitionCollection. Représente une collection d'objets OutlineCodeDefinition."
type: docs
weight: 1180
url: /fr/net/aspose.tasks/outlinecodedefinitioncollection/
---
## OutlineCodeDefinitionCollection class

Représente une collection d'objets [`OutlineCodeDefinition`](../outlinecodedefinition/).

```csharp
public class OutlineCodeDefinitionCollection : IList<OutlineCodeDefinition>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../aspose.tasks/outlinecodedefinitioncollection/count/) { get; } | Obtient le nombre d'éléments contenus dans cette collection. |
| [IsReadOnly](../../aspose.tasks/outlinecodedefinitioncollection/isreadonly/) { get; } | Obtient une valeur indiquant si cette collection est en lecture seule ; sinon, false. |
| [Item](../../aspose.tasks/outlinecodedefinitioncollection/item/) { get; set; } | Renvoie ou définit l'élément à l'index spécifié. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.tasks/outlinecodedefinitioncollection/add/)(OutlineCodeDefinition) | Ajoute l'élément spécifié à cette collection. |
| [Clear](../../aspose.tasks/outlinecodedefinitioncollection/clear/)() | Supprime tous les éléments de cette collection. |
| [Contains](../../aspose.tasks/outlinecodedefinitioncollection/contains/)(OutlineCodeDefinition) | Renvoie true si l'élément spécifié est trouvé dans cette collection ; sinon, false. |
| [CopyTo](../../aspose.tasks/outlinecodedefinitioncollection/copyto/)(OutlineCodeDefinition[], int) | Copie les éléments de cette collection dans le tableau spécifié, en commençant à l'index de tableau spécifié. |
| [GetEnumerator](../../aspose.tasks/outlinecodedefinitioncollection/getenumerator/)() | Renvoie un énumérateur pour cette collection. |
| [IndexOf](../../aspose.tasks/outlinecodedefinitioncollection/indexof/)(OutlineCodeDefinition) | Détermine l'index de l'élément spécifié dans cette collection. |
| [Insert](../../aspose.tasks/outlinecodedefinitioncollection/insert/)(int, OutlineCodeDefinition) | Insère l'élément spécifié à l'index spécifié. |
| [Remove](../../aspose.tasks/outlinecodedefinitioncollection/remove/)(OutlineCodeDefinition) | Supprime la première occurrence d'un objet spécifique de cette collection. |
| [RemoveAt](../../aspose.tasks/outlinecodedefinitioncollection/removeat/)(int) | Supprime un élément à l'index spécifié. |
| [ToList](../../aspose.tasks/outlinecodedefinitioncollection/tolist/)() | Convertit cet objet OutlineCodeDefinitionCollection en une liste d'objets [`OutlineCodeDefinition`](../outlinecodedefinition/). |

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

* class [OutlineCodeDefinition](../outlinecodedefinition/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


