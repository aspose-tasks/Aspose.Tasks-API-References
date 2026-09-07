---
title: "Classe TaskUtils"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.Util.TaskUtils classe. Classe di supporto che fornisce operazioni utili con i task"
type: docs
weight: 2770
url: /it/net/aspose.tasks.util/taskutils/
---
## TaskUtils class

Classe di supporto che fornisce operazioni utili sulle attività.

```csharp
public static class TaskUtils
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [Apply](../../aspose.tasks.util/taskutils/apply/)(Task, ITreeAlgorithm&lt;Task&gt;, int) | Applica l'algoritmo specificato a ogni task di un albero. |
| static [Filter](../../aspose.tasks.util/taskutils/filter/)(Task, ICondition&lt;Task&gt;) | Costruisce un nuovo albero di task che soddisfano la condizione. |
| static [Find](../../aspose.tasks.util/taskutils/find/)(Task, ICondition&lt;Task&gt;) | Trova un task che soddisfa la condizione in un albero di task. |
| static [TaskChildrenCount](../../aspose.tasks.util/taskutils/taskchildrencount/)(Task) | Calcola ricorsivamente il numero di task figli di un task attraverso tutti i livelli. |

## Esempi

Mostra come lavorare con un algoritmo ad albero.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// raccogli tutti i task del progetto
var coll = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, coll, 0);

// lavora con i task come con un semplice elenco
foreach (var task in coll.Tasks)
{
    Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
}
```

### Vedi anche

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


