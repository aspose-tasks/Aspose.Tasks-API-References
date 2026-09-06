---
title: "Task.SelectAllChildTasks"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Task. Récupère récursivement toutes les sous‑tâches de ce task"
type: docs
weight: 1400
url: /fr/net/aspose.tasks/task/selectallchildtasks/
---
## Task.SelectAllChildTasks method

Collecte récursivement toutes les tâches enfants de cette tâche.

```csharp
public IEnumerable<Task> SelectAllChildTasks()
```

### Valeur de retour

Une liste des sous‑tâches de ce task.

## Exemples

Montre comment itérer sur les sous‑tâches.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task 1");
task.Children.Add("Task 2");

foreach (var tsk in project.RootTask.SelectAllChildTasks())
{
    Console.WriteLine("{0} {1}", tsk.Get(Tsk.Id), tsk.Get(Tsk.Name));
}
```

### Voir aussi

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


