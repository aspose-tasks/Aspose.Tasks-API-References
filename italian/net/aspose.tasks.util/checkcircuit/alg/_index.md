---
title: "CheckCircuit.Alg"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo CheckCircuit. Verifica se l'oggetto specificato è già stato elaborato"
type: docs
weight: 20
url: /it/net/aspose.tasks.util/checkcircuit/alg/
---
## CheckCircuit.Alg method

Verifica se l'oggetto specificato è già stato elaborato.

```csharp
public override void Alg(Task el, int level)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| el | Attività | Oggetto da elaborare. |
| livello | Int32 | Livello del nodo dell'albero. |

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

* class [Task](../../../aspose.tasks/task/)
* class [CheckCircuit](../)
* namespace [Aspose.Tasks.Util](../../checkcircuit/)
* assembly [Aspose.Tasks](../../../)


