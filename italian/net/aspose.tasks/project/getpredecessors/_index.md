---
title: "Project.GetPredecessors"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo del progetto. Restituisce una collezione di collegamenti di attività che sono predecessori dell'attività specificata"
type: docs
weight: 1120
url: /it/net/aspose.tasks/project/getpredecessors/
---
## Project.GetPredecessors method

Restituisce una raccolta di collegamenti di attività che sono predecessori dell'attività specificata.

```csharp
public TaskLinkCollection GetPredecessors(Task task)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| attività | Attività | L'attività per cui ottenere i predecessori. |

### Valore di ritorno

Elenco dei predecessori [`TaskLink`](../../tasklink/).

## Esempi

Mostra come ottenere i predecessori per l'attività specifica.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");
var task = project.RootTask.Children.GetById(10);

var predecessors = project.GetPredecessors(task);

// Visualizza i nomi delle attività predecessore e successiva
foreach (var predecessor in predecessors)
{
    Console.WriteLine("Predecessor " + predecessor.PredTask.Get(Tsk.Name));
    Console.WriteLine("Successor " + predecessor.SuccTask.Get(Tsk.Name));
}
```

### Vedi anche

* class [TaskLinkCollection](../../tasklinkcollection/)
* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


