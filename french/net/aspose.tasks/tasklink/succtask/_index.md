---
title: "TaskLink.SuccTask"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété TaskLink. Obtient ou définit la tâche successeur"
type: docs
weight: 80
url: /fr/net/aspose.tasks/tasklink/succtask/
---
## TaskLink.SuccTask property

Obtient ou définit la tâche successeur.

```csharp
public Task SuccTask { get; set; }
```

## Exemples

Montre comment lire les liens de tâches du projet.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

// Afficher les noms des tâches prédécesseur et successeur
foreach (var taskLink in project.TaskLinks)
{
    Console.WriteLine("Predecessor: " + taskLink.PredTask.Get(Tsk.Name));
    Console.WriteLine("Successor: " + taskLink.SuccTask.Get(Tsk.Name));
    Console.WriteLine("Lag Format: " + taskLink.LagFormat);
    Console.WriteLine("Link Lag: " + taskLink.LinkLag);
    Console.WriteLine();
}
```

### Voir aussi

* class [Task](../../task/)
* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


