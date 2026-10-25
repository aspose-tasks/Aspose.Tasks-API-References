---
title: "Task.OutlineOutdent"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Task. Promouvoir une tâche dans le plan"
type: docs
weight: 1390
url: /fr/net/aspose.tasks/task/outlineoutdent/
---
## Task.OutlineOutdent method

Promouvoir une tâche dans l'outline.

```csharp
public void OutlineOutdent()
```

## Exemples

Montre comment désindenter une tâche.

```csharp
var project = new Project();
var task1 = project.RootTask.Children.Add("Parent");
var task2 = task1.Children.Add("Task");
Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));

// désindentez la tâche
task2.OutlineOutdent();

Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));
```

### Voir aussi

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


