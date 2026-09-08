---
title: "Task.Delete"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Task methode. Verwijdert een taak uit de takenverzameling van het bovenliggende project en al zijn toewijzingen"
type: docs
weight: 1320
url: /nl/net/aspose.tasks/task/delete/
---
## Task.Delete method

Verwijdert een taak uit de takenverzameling van het bovenliggende project en al haar toewijzingen.

```csharp
public void Delete()
```

## Voorbeelden

Toont hoe een taak te verwijderen.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Number of tasks: " + project.RootTask.Children.Count);

// verwijder een taak
task.Delete();

Console.WriteLine("Number of tasks: " + project.RootTask.Children.Count);
```

### Zie ook

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


