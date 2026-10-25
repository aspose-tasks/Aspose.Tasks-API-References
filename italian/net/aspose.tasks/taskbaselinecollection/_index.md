---
title: "Classe TaskBaselineCollection"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "La classe Aspose.Tasks.TaskBaselineCollection. Rappresenta una raccolta di oggetti TaskBaseline"
type: docs
weight: 2380
url: /it/net/aspose.tasks/taskbaselinecollection/
---
## TaskBaselineCollection class

Rappresenta una raccolta di oggetti [`TaskBaseline`](../taskbaseline/).

```csharp
public class TaskBaselineCollection : IList<TaskBaseline>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.tasks/taskbaselinecollection/count/) { get; } | Ottiene il numero di oggetti contenuti in questo oggetto TaskBaselineCollection. |
| [Item](../../aspose.tasks/taskbaselinecollection/item/) { get; set; } | Restituisce l'elemento all'indice specificato. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.tasks/taskbaselinecollection/add/)(TaskBaseline) | Questa è l'implementazione stub del metodo Add di ICollection, che lancia solo NotSupportedException |
| [GetEnumerator](../../aspose.tasks/taskbaselinecollection/getenumerator/)() | Restituisce un enumeratore per questa collezione. |
| [Remove](../../aspose.tasks/taskbaselinecollection/remove/)(TaskBaseline) | Rimuove la baseline da questa raccolta. |
| [ToList](../../aspose.tasks/taskbaselinecollection/tolist/)() | Converte l'oggetto TaskBaselineCollection in un elenco di oggetti [`TaskBaseline`](../taskbaseline/). |

## Esempi

Mostra come lavorare con le raccolte di baseline dei task.

```csharp
var project = new Project();

// crea baseline di progetto
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// stampa le baseline dei task
Console.WriteLine("Count of task baselines: " + task.Baselines.Count);
foreach (var baseline in task.Baselines)
{
    Console.WriteLine("Baseline duration: {0}", baseline.Duration);
    Console.WriteLine("Baseline start: {0}", baseline.Start);
    Console.WriteLine("Baseline finish: {0}", baseline.Finish);
}

// cancella tutte le baseline
List<TaskBaseline> baselines = task.Baselines.ToList();
for (var i = 0; i < baselines.Count; i++)
{
    task.Baselines.Remove(baselines[i]);
}
```

### Vedi anche

* class [TaskBaseline](../taskbaseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


