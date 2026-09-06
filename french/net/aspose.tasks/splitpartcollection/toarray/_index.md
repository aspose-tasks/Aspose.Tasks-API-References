---
title: "SplitPartCollection.ToArray"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode SplitPartCollection. Copie toutes les parties de la collection dans un nouveau tableau"
type: docs
weight: 40
url: /fr/net/aspose.tasks/splitpartcollection/toarray/
---
## SplitPartCollection.ToArray method

Copie toutes les parties de la collection dans un nouveau tableau.

```csharp
public SplitPart[] ToArray()
```

### Valeur de retour

Un tableau d'objets [`SplitPart`](../../splitpart/).

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


