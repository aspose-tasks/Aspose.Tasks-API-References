---
title: "Classe CheckCircuit"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Util.CheckCircuit. Verifica se un albero di task contiene un circuito"
type: docs
weight: 2680
url: /it/net/aspose.tasks.util/checkcircuit/
---
## CheckCircuit class

Verifica se un albero (di attività) contiene un circuito.

```csharp
public class CheckCircuit : TreeAlgorithmBase<Task>
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [CheckCircuit](checkcircuit/)() | Inizializza una nuova istanza della classe `CheckCircuit`. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [Alg](../../aspose.tasks.util/checkcircuit/alg/)(Task, int) | Verifica se l'oggetto specificato è già stato elaborato. |
| virtual [PostAlg](../../aspose.tasks.util/treealgorithmbase-1/postalg/)(Task, int) |  |
| virtual [PreAlg](../../aspose.tasks.util/treealgorithmbase-1/prealg/)(Task, int) |  |

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

* class [TreeAlgorithmBase&lt;T&gt;](../treealgorithmbase-1/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


