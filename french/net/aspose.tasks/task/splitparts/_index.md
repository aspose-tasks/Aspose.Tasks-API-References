---
title: "Task.SplitParts"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Task. Obtient une collection SplitPart qui représente les parties d'une tâche"
type: docs
weight: 1110
url: /fr/net/aspose.tasks/task/splitparts/
---
## Task.SplitParts property

Obtient une collection SplitPart qui représente les portions d'une tâche.

```csharp
public SplitPartCollection SplitParts { get; }
```

## Exemples

Montre comment afficher les parties découpées d'une tâche.

```csharp
var project = new Project(DataDir + "ViewSplitTasks.mpp");

// Accéder à la tâche 
var task = project.RootTask.Children.GetById(4);

// Afficher les parties découpées de la tâche
var collection = task.SplitParts;
foreach (var splitPart in collection)
{
    Console.WriteLine("Start: " + splitPart.Start + "\nFinish: " + splitPart.Finish + "\n");
}
```

### Voir aussi

* class [SplitPartCollection](../../splitpartcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


