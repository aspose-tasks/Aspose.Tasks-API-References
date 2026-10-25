---
title: "SplitPartCollection.Item"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété SplitPartCollection. Récupère une partie découpée d'une tâche à l'index donné"
type: docs
weight: 20
url: /fr/net/aspose.tasks/splitpartcollection/item/
---
## SplitPartCollection indexer

Récupère la partie découpée d'une tâche à l'index donné.

```csharp
public SplitPart this[int index] { get; set; }
```

| Paramètre | Description |
| --- | --- |
| index | L'index de la partie. |

### Valeur de retour

une partie découpée.

## Remarques

L'index commence à zéro. Retourne null si l'index est en dehors des limites du tableau.

## Exemples

Montre comment travailler avec les collections de parties découpées.

```csharp
var project = new Project(DataDir + "Splits.mpp");

var task = project.RootTask.Children.GetById(1);

// itérer sur les parties découpées
Console.WriteLine("Iterate over split parts");
Console.WriteLine("Split parts count:" + task.SplitParts.Count);
foreach (var splitPart in task.SplitParts)
{
    Console.WriteLine("Start: " + splitPart.Start);
    Console.WriteLine("Finish: " + splitPart.Finish);
}

// obtenir la partie par index
var split = task.SplitParts[0];
Console.WriteLine("Split start: " + split.Start);

// effectuer quelques opérations avec la première partie découpée de la tâche
```

### Voir aussi

* class [SplitPart](../../splitpart/)
* class [SplitPartCollection](../)
* namespace [Aspose.Tasks](../../splitpartcollection/)
* assembly [Aspose.Tasks](../../../)


