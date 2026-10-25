---
title: "TaskLink.LinkType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "TaskLink proprietà. Ottiene o imposta il tipo di collegamento"
type: docs
weight: 60
url: /it/net/aspose.tasks/tasklink/linktype/
---
## TaskLink.LinkType property

Ottiene o imposta il tipo di collegamento.

```csharp
public TaskLinkType LinkType { get; set; }
```

## Esempi

Mostra come ottenere/impostare il tipo di collegamento di un collegamento di attività.

```csharp
var project = new Project();

// Aggiungi nuove attività
var pred = project.RootTask.Children.Add("Task 1");
var succ = project.RootTask.Children.Add("Task 2");

// Collega le attività con il tipo di collegamento impostato su Inizio a Inizio
var newLink = project.TaskLinks.Add(pred, succ);
newLink.LinkType = TaskLinkType.StartToStart;

foreach (var link in project.TaskLinks)
{
    Console.WriteLine("Task Link Type: " + link.LinkType.ToString());
}
```

### Vedi anche

* enum [TaskLinkType](../../tasklinktype/)
* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


