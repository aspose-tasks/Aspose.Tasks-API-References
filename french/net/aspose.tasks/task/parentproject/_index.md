---
title: "Task.ParentProject"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Task. Obtient le projet parent d'une tâche"
type: docs
weight: 930
url: /fr/net/aspose.tasks/task/parentproject/
---
## Task.ParentProject property

Obtient le projet parent d'une tâche.

```csharp
public Project ParentProject { get; }
```

## Remarques

Appelez Project.UpdateReferences pour mettre à jour ces propriétés.

## Exemples

Montre comment utiliser le projet parent d'une tâche.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Parent");

// définissez une durée pour la tâche en utilisant le type d'unité de temps par défaut du projet.
task.Set(Tsk.Duration, task.ParentProject.GetDuration(1));

Console.WriteLine(task.Get(Tsk.Duration));
```

### Voir aussi

* class [Project](../../project/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


