---
title: "Task.ParentTask"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Task. Obtient la tâche parente d'une tâche"
type: docs
weight: 940
url: /fr/net/aspose.tasks/task/parenttask/
---
## Task.ParentTask property

Obtient la tâche parente d'une tâche.

```csharp
public Task ParentTask { get; }
```

## Exemples

Montre comment utiliser la tâche parente d'une tâche.

```csharp
var project = new Project();
var parent = project.RootTask.Children.Add("Parent");
var child1 = parent.Children.Add("Child1");
var child2 = child1.ParentTask.Children.Add("Child2");

Console.WriteLine("Is parent is equal to the root task: " + child2.ParentTask.Equals(parent));
```

### Voir aussi

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


