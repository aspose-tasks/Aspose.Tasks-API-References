---
title: "Classe SplitPartCollection"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.SplitPartCollection. Collection qui représente les portions d'une tâche."
type: docs
weight: 2300
url: /fr/net/aspose.tasks/splitpartcollection/
---
## SplitPartCollection class

Collection qui représente les portions d'une tâche.

```csharp
public class SplitPartCollection : IList<SplitPart>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../aspose.tasks/splitpartcollection/count/) { get; } | Obtient le nombre de parties dans la collection. |
| [Item](../../aspose.tasks/splitpartcollection/item/) { get; set; } | Récupère la partie découpée d'une tâche à l'index donné. |

## Méthodes

| Nom | Description |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/splitpartcollection/getenumerator/)() | Renvoie un énumérateur pour cette collection. |
| [ToArray](../../aspose.tasks/splitpartcollection/toarray/)() | Copie toutes les parties de la collection dans un nouveau tableau. |

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

* class [SplitPart](../splitpart/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


