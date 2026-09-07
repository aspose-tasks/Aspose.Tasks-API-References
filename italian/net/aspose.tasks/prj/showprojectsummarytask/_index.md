---
title: "Prj.ShowProjectSummaryTask"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Prj field. Determina se visualizzare le informazioni di riepilogo di un intero progetto in una singola riga con la propria barra di attività di riepilogo nella parte superiore della vista Gantt Chart"
type: docs
weight: 640
url: /it/net/aspose.tasks/prj/showprojectsummarytask/
---
## Prj.ShowProjectSummaryTask field

Determina se visualizzare le informazioni di riepilogo di un intero progetto su una singola riga con la propria barra di attività di riepilogo nella parte superiore della visualizzazione Gantt.

```csharp
public static readonly Key<bool, PrjKey> ShowProjectSummaryTask;
```

## Esempi

Mostra come leggere/scrivere la proprietà Prj.ShowProjectSummaryTask.

```csharp
var project = new Project();

project.Set(Prj.ShowProjectSummaryTask, true);

Console.WriteLine("Show Project Summary Task: " + project.Get(Prj.ShowProjectSummaryTask));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


