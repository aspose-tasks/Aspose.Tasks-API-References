---
title: "Task.Baselines"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Task. Ottiene o imposta la collezione dei valori di baseline del task"
type: docs
weight: 130
url: /it/net/aspose.tasks/task/baselines/
---
## Task.Baselines property

Ottiene o imposta la collezione dei valori di baseline dell'attività.

```csharp
public TaskBaselineCollection Baselines { get; set; }
```

## Esempi

Mostra come leggere le baseline del task.

```csharp
var project = new Project();

// imposta una baseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// Visualizza la durata della baseline dell'attività
foreach (var baseline in task.Baselines)
{
    Console.WriteLine("Baseline duration is 1 day: {0}", baseline.Duration.ToString().Equals("1 day"));
    Console.WriteLine("BaselineStart is same as Task Start: {0}", baseline.Start.Equals(task.Get(Tsk.Start)));
    Console.WriteLine("BaselineFinish is same as Task Finish: {0}", baseline.Finish.Equals(task.Get(Tsk.Finish)));
}
```

### Vedi anche

* class [TaskBaselineCollection](../../taskbaselinecollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


