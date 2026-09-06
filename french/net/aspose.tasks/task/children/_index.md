---
title: "Task.Children"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Task. Obtient une collection de tâches enfants de cet objet. Objet TaskCollection qui représente les tâches enfants"
type: docs
weight: 190
url: /fr/net/aspose.tasks/task/children/
---
## Task.Children property

Obtient une collection de sous-tâches de cet objet. Objet TaskCollection qui représente les tâches enfants.

```csharp
public TaskCollection Children { get; }
```

## Exemples

Montre comment utiliser la collection de tâches pour ajouter une tâche.

```csharp
var project = new Project();

// Ajouter une tâche, une sous‑tâche et enregistrer le projet
var task = project.RootTask.Children.Add("Summary1");
task.Children.Add("Subtask1");
project.Save(OutDir + "CreateTasks_out.xml", SaveFileFormat.Xml);
```

### Voir aussi

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


