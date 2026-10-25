---
title: "TaskLink.LinkLag"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété TaskLink. Obtient ou définit le retard en dixièmes de minute ou en pourcentage"
type: docs
weight: 40
url: /fr/net/aspose.tasks/tasklink/linklag/
---
## TaskLink.LinkLag property

Obtient ou définit le retard en dixièmes de minute ou en pourcentage.

```csharp
public int LinkLag { get; set; }
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

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


