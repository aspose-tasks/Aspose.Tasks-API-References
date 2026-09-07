---
title: "TreeAlgorithmBase1.PreAlg"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo TreeAlgorithmBase. Chiamato prima dell'elaborazione di un nodo di un albero"
type: docs
weight: 30
url: /it/net/aspose.tasks.util/treealgorithmbase-1/prealg/
---
## TreeAlgorithmBase&lt;T&gt;.PreAlg method

Chiamato prima dell'elaborazione di un nodo di un albero.

```csharp
public virtual void PreAlg(T el, int level)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| el | T | Nodo da elaborare. |
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

* class [TreeAlgorithmBase&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../treealgorithmbase-1/)
* assembly [Aspose.Tasks](../../../)


