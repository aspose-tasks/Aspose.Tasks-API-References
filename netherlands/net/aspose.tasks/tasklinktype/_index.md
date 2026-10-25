---
title: "Enum TaskLinkType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.TaskLinkType enum. Specificeert het type taakafhankelijkheid"
type: docs
weight: 2440
url: /nl/net/aspose.tasks/tasklinktype/
---
## TaskLinkType enumeration

Specificeert het type van taakafhankelijkheid.

```csharp
public enum TaskLinkType
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| FinishToFinish | `0` | Finish-Finish relatie |
| FinishToStart | `1` | Finish-Start relatie |
| StartToFinish | `2` | Start-Finish relatie |
| StartToStart | `3` | Start-Start relatie |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


