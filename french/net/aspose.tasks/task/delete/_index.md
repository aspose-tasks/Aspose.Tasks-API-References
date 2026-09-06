---
title: "Task.Delete"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Task. Supprime une tâche de la collection des tâches du projet parent et de toutes ses affectations"
type: docs
weight: 1320
url: /fr/net/aspose.tasks/task/delete/
---
## Task.Delete method

Supprime une tâche de la collection des tâches du projet parent et de toutes ses affectations.

```csharp
public void Delete()
```

## Exemples

Montre comment supprimer une tâche.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Number of tasks: " + project.RootTask.Children.Count);

// supprimer une tâche
task.Delete();

Console.WriteLine("Number of tasks: " + project.RootTask.Children.Count);
```

### Voir aussi

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


