---
title: "Classe TaskLink"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.TaskLink. Rappresenta un collegamento predecessore"
type: docs
weight: 2410
url: /it/net/aspose.tasks/tasklink/
---
## TaskLink class

Rappresenta un collegamento predecessore.

```csharp
public sealed class TaskLink : IEquatable<TaskLink>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CrossProjectName](../../aspose.tasks/tasklink/crossprojectname/) { get; set; } | Ottiene o imposta il progetto predecessore esterno. |
| [IsCrossProject](../../aspose.tasks/tasklink/iscrossproject/) { get; set; } | Ottiene o imposta un valore che indica se un predecessore fa parte di un altro progetto. |
| [LagFormat](../../aspose.tasks/tasklink/lagformat/) { get; set; } | Ottiene o imposta il formato per esprimere il ritardo. |
| [LinkLag](../../aspose.tasks/tasklink/linklag/) { get; set; } | Ottiene o imposta il ritardo in decimi di minuto o in percentuale. |
| [LinkLagTimeSpan](../../aspose.tasks/tasklink/linklagtimespan/) { get; set; } | Ottiene o imposta la durata del ritardo, a seconda del LagFormat. |
| [LinkType](../../aspose.tasks/tasklink/linktype/) { get; set; } | Ottiene o imposta il tipo di collegamento. |
| [PredTask](../../aspose.tasks/tasklink/predtask/) { get; set; } | Ottiene o imposta l'attività predecessore. |
| [SuccTask](../../aspose.tasks/tasklink/succtask/) { get; set; } | Ottiene o imposta l'attività successiva. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [Equals](../../aspose.tasks/tasklink/equals/#equals_1)(object) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| [Equals](../../aspose.tasks/tasklink/equals/#equals)(TaskLink) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| override [GetHashCode](../../aspose.tasks/tasklink/gethashcode/)() | Restituisce un valore di codice hash per l'istanza della classe `TaskLink`. |
| override [ToString](../../aspose.tasks/tasklink/tostring/)() | Restituisce la rappresentazione stringa di un TaskLink. I dettagli esatti della rappresentazione non sono specificati e possono cambiare. |

## Esempi

Mostra come leggere i collegamenti delle attività del progetto.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

// Visualizza i nomi delle attività predecessore e successiva
foreach (var taskLink in project.TaskLinks)
{
    Console.WriteLine("Predecessor: " + taskLink.PredTask.Get(Tsk.Name));
    Console.WriteLine("Successor: " + taskLink.SuccTask.Get(Tsk.Name));
    Console.WriteLine("Lag Format: " + taskLink.LagFormat);
    Console.WriteLine("Link Lag: " + taskLink.LinkLag);
    Console.WriteLine();
}
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


