---
title: "TaskUtils.TaskChildrenCount"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode TaskUtils. Calcule récursivement le nombre de tâches enfants à travers tous les niveaux"
type: docs
weight: 40
url: /fr/net/aspose.tasks.util/taskutils/taskchildrencount/
---
## TaskUtils.TaskChildrenCount method

Calcule récursivement le nombre de sous‑tâches d'une tâche à tous les niveaux.

```csharp
public static int TaskChildrenCount(Task task)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| tâche | Tâche | La tâche dont les enfants sont calculés. |

### Valeur de retour

Le nombre d'enfants.

## Exemples

Montre comment utiliser la méthode &lt;see cref="Aspose.Tasks.Util.TaskUtils.TaskChildrenCount" /&gt;.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// calcule récursivement le nombre de tâches enfants d'une tâche à travers tous les niveaux
var count = TaskUtils.TaskChildrenCount(project.RootTask);

Console.WriteLine("Number of tasks: " + count);
```

### Voir aussi

* class [Task](../../../aspose.tasks/task/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


