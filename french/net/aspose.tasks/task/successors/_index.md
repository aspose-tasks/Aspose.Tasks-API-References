---
title: "Task.Successors"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Task. Obtient un objet TaskCollection qui contient tous les successeurs de cet objet Task"
type: docs
weight: 1200
url: /fr/net/aspose.tasks/task/successors/
---
## Task.Successors property

Obtient un objet [`TaskCollection`](../../taskcollection/) qui contient tous les successeurs de cet objet Task.

```csharp
public TaskCollection Successors { get; }
```

### Valeur de retour

Instance en lecture seule de la classe [`TaskCollection`](../../taskcollection/).

## Exemples

Montre comment lire les successeurs d'une tâche.

```csharp
var project = new Project();
var pred = project.RootTask.Children.Add("Predecessor");
var succ = project.RootTask.Children.Add("Successor");

project.TaskLinks.Add(pred, succ);

foreach (var successor in pred.Successors)
{
    Console.WriteLine("{0} {1}", successor.Get(Tsk.Id), successor.Get(Tsk.Name));
}
```

### Voir aussi

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


