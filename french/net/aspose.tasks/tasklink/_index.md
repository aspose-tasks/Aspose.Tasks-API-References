---
title: "Classe TaskLink"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.TaskLink. Représente un lien de prédécesseur"
type: docs
weight: 2410
url: /fr/net/aspose.tasks/tasklink/
---
## TaskLink class

Représente un lien de prédécesseur.

```csharp
public sealed class TaskLink : IEquatable<TaskLink>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [CrossProjectName](../../aspose.tasks/tasklink/crossprojectname/) { get; set; } | Obtient ou définit le projet prédécesseur externe. |
| [IsCrossProject](../../aspose.tasks/tasklink/iscrossproject/) { get; set; } | Obtient ou définit une valeur indiquant si un prédécesseur fait partie d’un autre projet. |
| [LagFormat](../../aspose.tasks/tasklink/lagformat/) { get; set; } | Obtient ou définit le format d’expression du retard. |
| [LinkLag](../../aspose.tasks/tasklink/linklag/) { get; set; } | Obtient ou définit le retard en dixièmes de minute ou en pourcentage. |
| [LinkLagTimeSpan](../../aspose.tasks/tasklink/linklagtimespan/) { get; set; } | Obtient ou définit la durée du retard, selon le LagFormat. |
| [LinkType](../../aspose.tasks/tasklink/linktype/) { get; set; } | Obtient ou définit le type d’un lien. |
| [PredTask](../../aspose.tasks/tasklink/predtask/) { get; set; } | Obtient ou définit la tâche prédécesseur. |
| [SuccTask](../../aspose.tasks/tasklink/succtask/) { get; set; } | Obtient ou définit la tâche successeur. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [Equals](../../aspose.tasks/tasklink/equals/#equals_1)(object) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| [Equals](../../aspose.tasks/tasklink/equals/#equals)(TaskLink) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| override [GetHashCode](../../aspose.tasks/tasklink/gethashcode/)() | Renvoie une valeur de code de hachage pour l’instance de la classe `TaskLink`. |
| override [ToString](../../aspose.tasks/tasklink/tostring/)() | Renvoie la représentation sous forme de chaîne d’un TaskLink. Les détails exacts de la représentation ne sont pas spécifiés et peuvent changer. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


