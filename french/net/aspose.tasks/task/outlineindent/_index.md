---
title: "Task.OutlineIndent"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Task. Indente une tâche dans le plan"
type: docs
weight: 1380
url: /fr/net/aspose.tasks/task/outlineindent/
---
## Task.OutlineIndent method

Indente une tâche dans l'outline.

```csharp
public void OutlineIndent()
```

## Exemples

Montre comment indenter une tâche.

```csharp
var project = new Project();
var task1 = project.RootTask.Children.Add("Parent");
var task2 = project.RootTask.Children.Add("Task");
Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));

// indenter la tâche
task2.OutlineIndent();

Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));
```

### Voir aussi

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


