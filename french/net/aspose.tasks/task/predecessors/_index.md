---
title: "Task.Predecessors"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Task. Obtient un objet TaskCollection qui contient tous les antécédents de cet objet Task"
type: docs
weight: 980
url: /fr/net/aspose.tasks/task/predecessors/
---
## Task.Predecessors property

Obtient un objet [`TaskCollection`](../../taskcollection/) qui contient tous les antécédents de cet objet Task.

```csharp
public TaskCollection Predecessors { get; }
```

### Valeur de retour

Instance en lecture seule de la classe [`TaskCollection`](../../taskcollection/).

## Exemples

Montre comment lire les antécédents d'une tâche.

```csharp
var project = new Project();
var pred = project.RootTask.Children.Add("Predecessor");
var succ = project.RootTask.Children.Add("Successor");

project.TaskLinks.Add(pred, succ);

foreach (var predecessor in succ.Predecessors)
{
    Console.WriteLine("{0} {1}", predecessor.Get(Tsk.Id), predecessor.Get(Tsk.Name));
}
```

### Voir aussi

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


