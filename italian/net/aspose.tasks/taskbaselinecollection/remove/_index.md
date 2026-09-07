---
title: "TaskBaselineCollection.Remove"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo TaskBaselineCollection. Rimuove la baseline da questa collezione"
type: docs
weight: 50
url: /it/net/aspose.tasks/taskbaselinecollection/remove/
---
## TaskBaselineCollection.Remove method

Rimuove la baseline da questa raccolta.

```csharp
public bool Remove(TaskBaseline item)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| elemento | TaskBaseline | L'elemento da rimuovere. |

### Valore di ritorno

true se l'elemento è stato rimosso con successo; altrimenti, false

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

* class [TaskBaseline](../../taskbaseline/)
* class [TaskBaselineCollection](../)
* namespace [Aspose.Tasks](../../taskbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


