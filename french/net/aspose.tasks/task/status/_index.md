---
title: "Task.Status"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Task. Obtient le statut de la tâche"
type: docs
weight: 1160
url: /fr/net/aspose.tasks/task/status/
---
## Task.Status property

Obtient le statut de la tâche.

```csharp
public TaskStatus Status { get; }
```

## Exemples

Montre comment obtenir le statut de la tâche.

```csharp
var project = new Project(DataDir + "TaskPercentageCompletion.mpp");

// La date de statut du projet doit être définie car le calcul du statut utilise la date de statut.
project.StatusDate = new DateTime(2010, 7, 9, 15, 0, 0);
foreach (var task in project.EnumerateAllChildTasks())
{
    Console.WriteLine("{0} - {1}", task.Name, task.Status);
}
```

### Voir aussi

* enum [TaskStatus](../../taskstatus/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


