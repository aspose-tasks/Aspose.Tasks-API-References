---
title: "TaskLink.LagFormat"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété TaskLink. Obtient ou définit le format d'expression du retard"
type: docs
weight: 30
url: /fr/net/aspose.tasks/tasklink/lagformat/
---
## TaskLink.LagFormat property

Obtient ou définit le format d’expression du retard.

```csharp
public TimeUnitType LagFormat { get; set; }
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

* enum [TimeUnitType](../../timeunittype/)
* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


