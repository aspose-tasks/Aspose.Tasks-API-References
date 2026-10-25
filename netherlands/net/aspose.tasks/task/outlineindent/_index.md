---
title: "Task.OutlineIndent"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Task-methode. Inspringt een taak in de outline"
type: docs
weight: 1380
url: /nl/net/aspose.tasks/task/outlineindent/
---
## Task.OutlineIndent method

Voegt een inspringing toe aan een taak in de outline.

```csharp
public void OutlineIndent()
```

## Voorbeelden

Toont hoe een taak in te springen.

```csharp
var project = new Project();
var task1 = project.RootTask.Children.Add("Parent");
var task2 = project.RootTask.Children.Add("Task");
Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));

// inspringen van de taak
task2.OutlineIndent();

Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));
```

### Zie ook

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


