---
title: "Classe ChildTasksCollector"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Util.ChildTasksCollector. Raccoglie tutti i task figli"
type: docs
weight: 2690
url: /it/net/aspose.tasks.util/childtaskscollector/
---
## ChildTasksCollector class

Raccoglie tutte le attività figlio.

```csharp
public class ChildTasksCollector : TreeAlgorithmBase<Task>
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [ChildTasksCollector](childtaskscollector/)() | Inizializza una nuova istanza della classe `ChildTasksCollector`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Tasks](../../aspose.tasks.util/childtaskscollector/tasks/) { get; } | Ottiene un elenco di oggetti figli raccolti (task). |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [Alg](../../aspose.tasks.util/childtaskscollector/alg/)(Task, int) | Elabora l'oggetto specificato. |
| virtual [PostAlg](../../aspose.tasks.util/treealgorithmbase-1/postalg/)(Task, int) |  |
| virtual [PreAlg](../../aspose.tasks.util/treealgorithmbase-1/prealg/)(Task, int) |  |

## Esempi

Mostra come iterare su tutti i task di un progetto come una semplice lista.

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Analizza tutti i task raccolti
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### Vedi anche

* class [TreeAlgorithmBase&lt;T&gt;](../treealgorithmbase-1/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


