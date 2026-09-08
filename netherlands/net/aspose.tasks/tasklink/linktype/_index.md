---
title: "TaskLink.LinkType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TaskLink eigenschap. Haalt het type van een koppeling op of stelt dit in"
type: docs
weight: 60
url: /nl/net/aspose.tasks/tasklink/linktype/
---
## TaskLink.LinkType property

Haalt een waarde op of stelt deze in voor het type van een koppeling.

```csharp
public TaskLinkType LinkType { get; set; }
```

## Voorbeelden

Toont hoe een linktype van een taaklink opgehaald/ingesteld wordt.

```csharp
var project = new Project();

// Voeg nieuwe taken toe
var pred = project.RootTask.Children.Add("Task 1");
var succ = project.RootTask.Children.Add("Task 2");

// Koppel taken met linktype ingesteld op Start naar Start
var newLink = project.TaskLinks.Add(pred, succ);
newLink.LinkType = TaskLinkType.StartToStart;

foreach (var link in project.TaskLinks)
{
    Console.WriteLine("Task Link Type: " + link.LinkType.ToString());
}
```

### Zie ook

* enum [TaskLinkType](../../tasklinktype/)
* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


