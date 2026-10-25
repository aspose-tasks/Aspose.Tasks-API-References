---
title: "Task.OutlineOutdent"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Task methode. Promoot een taak in de outline"
type: docs
weight: 1390
url: /nl/net/aspose.tasks/task/outlineoutdent/
---
## Task.OutlineOutdent method

Promoveert een taak in de outline.

```csharp
public void OutlineOutdent()
```

## Voorbeelden

Toont hoe een taak uit te laten inspringen.

```csharp
var project = new Project();
var task1 = project.RootTask.Children.Add("Parent");
var task2 = task1.Children.Add("Task");
Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));

// laat de taak uit inspringen
task2.OutlineOutdent();

Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));
```

### Zie ook

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


