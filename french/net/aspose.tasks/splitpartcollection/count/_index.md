---
title: "SplitPartCollection.Count"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété SplitPartCollection. Obtient le nombre de parties dans la collection"
type: docs
weight: 10
url: /fr/net/aspose.tasks/splitpartcollection/count/
---
## SplitPartCollection.Count property

Obtient le nombre de parties dans la collection.

```csharp
public int Count { get; }
```

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

* class [SplitPartCollection](../)
* namespace [Aspose.Tasks](../../splitpartcollection/)
* assembly [Aspose.Tasks](../../../)


