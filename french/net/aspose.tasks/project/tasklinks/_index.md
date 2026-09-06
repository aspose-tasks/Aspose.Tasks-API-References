---
title: "Project.TaskLinks"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Project property. Obtient l'objet TaskLinkCollection"
type: docs
weight: 930
url: /fr/net/aspose.tasks/project/tasklinks/
---
## Project.TaskLinks property

Obtient l'objet [`TaskLinkCollection`](../../tasklinkcollection/).

```csharp
public TaskLinkCollection TaskLinks { get; }
```

## Exemples

Montre comment créer des liens de tâches.

```csharp
var project = new Project();

// Ajouter de nouvelles tâches
var pred = project.RootTask.Children.Add("Task 1");
var succ = project.RootTask.Children.Add("Task 2");

// Lier les tâches
project.TaskLinks.Add(pred, succ);

foreach (var link in project.TaskLinks)
{
    Console.WriteLine("Predecessor Task: " + link.PredTask);
    Console.WriteLine("Successor Task: " + link.SuccTask);
    Console.WriteLine("LagFormat: " + link.LagFormat);
    Console.WriteLine("LinkType: " + link.LinkType);
    Console.WriteLine("LinkLag: " + link.LinkLag);
    Console.WriteLine("CrossProjectName: " + link.CrossProjectName);
    Console.WriteLine("IsCrossProject: " + link.IsCrossProject);
}
```

### Voir aussi

* class [TaskLinkCollection](../../tasklinkcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


