---
title: "TaskLink.LinkType"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété TaskLink. Obtient ou définit le type d'un lien"
type: docs
weight: 60
url: /fr/net/aspose.tasks/tasklink/linktype/
---
## TaskLink.LinkType property

Obtient ou définit le type d’un lien.

```csharp
public TaskLinkType LinkType { get; set; }
```

## Exemples

Montre comment obtenir/définir un type de lien d'un lien de tâche.

```csharp
var project = new Project();

// Ajouter de nouvelles tâches
var pred = project.RootTask.Children.Add("Task 1");
var succ = project.RootTask.Children.Add("Task 2");

// Lier des tâches avec le type de lien défini sur Start to Start
var newLink = project.TaskLinks.Add(pred, succ);
newLink.LinkType = TaskLinkType.StartToStart;

foreach (var link in project.TaskLinks)
{
    Console.WriteLine("Task Link Type: " + link.LinkType.ToString());
}
```

### Voir aussi

* enum [TaskLinkType](../../tasklinktype/)
* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


