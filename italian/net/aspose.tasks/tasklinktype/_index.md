---
title: "Enum TaskLinkType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.TaskLinkType. Specifica il tipo di dipendenza tra attività"
type: docs
weight: 2440
url: /it/net/aspose.tasks/tasklinktype/
---
## TaskLinkType enumeration

Specifica il tipo di dipendenza delle attività.

```csharp
public enum TaskLinkType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| FinishToFinish | `0` | Relazione Fine-Fine |
| FinishToStart | `1` | Relazione Fine-Inizio |
| StartToFinish | `2` | Relazione Inizio-Fine |
| StartToStart | `3` | Relazione Inizio-Inizio |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


