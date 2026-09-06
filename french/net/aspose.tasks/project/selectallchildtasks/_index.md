---
title: "Project.SelectAllChildTasks"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Project. Récupère récursivement toutes les sous‑tâches de la tâche racine"
type: docs
weight: 1230
url: /fr/net/aspose.tasks/project/selectallchildtasks/
---
## Project.SelectAllChildTasks method

Collecte récursivement toutes les sous‑tâches de la tâche racine.

```csharp
public IEnumerable<Task> SelectAllChildTasks()
```

### Valeur de retour

La collection de tâches.

## Exemples

Montre comment renuméroter les codes WBS des tâches sélectionnées.

```csharp
var project = new Project(DataDir + "RenumberExample.mpp");

var tasks = new List<Task>(project.RootTask.SelectAllChildTasks());

Console.WriteLine("WBS codes before: ");

// sortie : ""; "1"; "2"; "4"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}

project.RenumberWBSCode(new List<int> { 1, 2, 3 });

Console.WriteLine("\nWBS codes after: ");

// sortie : ""; "1"; "2"; "3"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}
```

### Voir aussi

* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


