---
title: "Project.GetPredecessors"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode du projet. Retourne une collection de liens de tâches qui sont les prédécesseurs de la tâche spécifiée"
type: docs
weight: 1120
url: /fr/net/aspose.tasks/project/getpredecessors/
---
## Project.GetPredecessors method

Renvoie une collection de liens de tâches qui sont les prédécesseurs de la tâche spécifiée.

```csharp
public TaskLinkCollection GetPredecessors(Task task)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| tâche | Tâche | La tâche pour laquelle obtenir les prédécesseurs. |

### Valeur de retour

Liste des prédécesseurs [`TaskLink`](../../tasklink/).

## Exemples

Montre comment obtenir les prédécesseurs pour la tâche spécifique.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");
var task = project.RootTask.Children.GetById(10);

var predecessors = project.GetPredecessors(task);

// Afficher les noms des tâches prédécesseur et successeur
foreach (var predecessor in predecessors)
{
    Console.WriteLine("Predecessor " + predecessor.PredTask.Get(Tsk.Name));
    Console.WriteLine("Successor " + predecessor.SuccTask.Get(Tsk.Name));
}
```

### Voir aussi

* class [TaskLinkCollection](../../tasklinkcollection/)
* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


