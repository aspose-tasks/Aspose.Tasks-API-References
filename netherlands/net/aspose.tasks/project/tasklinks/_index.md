---
title: "Project.TaskLinks"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Projecteigenschap. Haalt TaskLinkCollection‑object op"
type: docs
weight: 930
url: /nl/net/aspose.tasks/project/tasklinks/
---
## Project.TaskLinks property

Haalt [`TaskLinkCollection`](../../tasklinkcollection/)‑object op.

```csharp
public TaskLinkCollection TaskLinks { get; }
```

## Voorbeelden

Toont hoe taakkoppelingen te maken.

```csharp
var project = new Project();

// Voeg nieuwe taken toe
var pred = project.RootTask.Children.Add("Task 1");
var succ = project.RootTask.Children.Add("Task 2");

// Taken koppelen
project.TaskLinks.Add(pred, succ);

foreach (var link in project.TaskLinks)
{
    Console.WriteLine("Predecessor Task: " + link.PredTask);
    Console.WriteLine("Successor Task: " + link.SuccTask);
    Console.WriteLine("LagFormat: " + link.LagFormat);
    Console.WriteLine("LinkType: " + link.LinkType);
    Console.WriteLine("LinkLag: " + link.LinkLag);
    Console.WriteLine("CrossProjectName: " + link.CrossProjectName);
    Console.WriteLine("IsCrossProject: " + link.IsCrossProject);
}
```

### Zie ook

* class [TaskLinkCollection](../../tasklinkcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


