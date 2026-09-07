---
title: "CheckCircuit.CheckCircuit"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Costruttore di CheckCircuit. Inizializza una nuova istanza della classe CheckCircuit"
type: docs
weight: 10
url: /it/net/aspose.tasks.util/checkcircuit/checkcircuit/
---
## CheckCircuit constructor

Inizializza una nuova istanza della classe [`CheckCircuit`](../).

```csharp
public CheckCircuit()
```

## Esempi

Mostra come rilevare la struttura del progetto rotta.

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

// verifica la struttura del progetto.
// Il <see cref=\"TasksException\"> verrà generato se la struttura del progetto è errata.
try
{
    TaskUtils.Apply(project.RootTask, new CheckCircuit(), 0);
}
catch (TasksException ex)
{
    Console.WriteLine(ex);
}
```

### Vedi anche

* class [CheckCircuit](../)
* namespace [Aspose.Tasks.Util](../../checkcircuit/)
* assembly [Aspose.Tasks](../../../)


