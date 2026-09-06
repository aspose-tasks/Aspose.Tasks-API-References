---
title: "Classe OutlineCode"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.OutlineCode. Représente une valeur d'un code de plan"
type: docs
weight: 1150
url: /fr/net/aspose.tasks/outlinecode/
---
## OutlineCode class

Représente une valeur d'un code de plan.

```csharp
public class OutlineCode
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [OutlineCode](outlinecode/#constructor)() | Initialise une nouvelle instance de la classe `OutlineCode`. |
| [OutlineCode](outlinecode/#constructor_1)(OutlineCodeDefinition, OutlineValue) | Initialise une nouvelle instance de la classe `OutlineCode` en utilisant le Outline Code spécifié et l'une de ses valeurs. |

## Propriétés

| Nom | Description |
| --- | --- |
| [FieldId](../../aspose.tasks/outlinecode/fieldid/) { get; set; } | Obtient ou définit la valeur numérique du champ personnalisé Id du projet. |
| [ValueGuid](../../aspose.tasks/outlinecode/valueguid/) { get; set; } | Obtient ou définit le GUID de la valeur dans la liste de valeurs. Le ValueGuid correspond au FieldGuid dans la liste de valeurs. |
| [ValueId](../../aspose.tasks/outlinecode/valueid/) { get; set; } | Obtient ou définit l'Id dans la liste de valeurs associé à la définition dans la collection de codes de plan. |

## Remarques

Deux éléments de données sont nécessaires - un pointeur vers la table de codes de plan spécifiée par le FieldId, et la valeur spécifiée soit par le ValueId soit par le pointeur ValueGuid vers la liste de valeurs.

## Exemples

Montre comment lire les codes de plan d'une tâche.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// lire les codes de plan
foreach (var task in project.RootTask.SelectAllChildTasks())
{
    if (task.OutlineCodes.Count <= 0)
    {
        continue;
    }

    Console.WriteLine("Print outline codes of the task: " + task.Get(Tsk.Name));
    foreach (var value in task.OutlineCodes)
    {
        Console.WriteLine("  Field Id: " + value.FieldId);
        Console.WriteLine("  Value Guid: " + value.ValueGuid);
        Console.WriteLine("  Value Id: " + value.ValueId);
    }
}
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


