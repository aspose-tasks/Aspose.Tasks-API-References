---
title: "Task.Clone"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Task. Crée une copie complète d'un task sans sous‑tâches"
type: docs
weight: 1310
url: /fr/net/aspose.tasks/task/clone/
---
## Task.Clone method

Crée une copie complète d'une tâche sans sous‑tâches.

```csharp
public object Clone()
```

### Valeur de retour

Copie d'une tâche créée.

## Exemples

Montre comment cloner une tâche.

```csharp
var project = new Project();

var originalTask = project.RootTask.Children.Add("Task");
var cloneTask = (Task)originalTask.Clone();

Console.WriteLine("Are tasks equal: " + cloneTask.Equals(originalTask));
```

### Voir aussi

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


