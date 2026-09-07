---
title: "TaskBaseline.Finish"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà TaskBaseline. Ottiene o imposta la data di fine pianificata dell'attività quando la baseline è stata salvata"
type: docs
weight: 40
url: /it/net/aspose.tasks/taskbaseline/finish/
---
## TaskBaseline.Finish property

Ottiene o imposta la data di fine programmata dell'attività quando è stata salvata la baseline.

```csharp
public DateTime Finish { get; set; }
```

## Esempi

Mostra come accedere a informazioni sulla baseline.

```csharp
var project = new Project();

// Creazione di TaskBaseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// Visualizza la durata della baseline dell'attività
var baseline = task.Baselines.ToList()[0];
Console.WriteLine("Baseline Start: {0}", baseline.Start);
Console.WriteLine("Baseline duration: {0}", baseline.Duration);
Console.WriteLine("Baseline duration format: {0}", baseline.Duration.TimeUnit);
Console.WriteLine("Is it estimated duration?: {0}", baseline.EstimatedDuration);
Console.WriteLine("Baseline Finish: {0}", baseline.Finish);

// valore che indica se questa è una Baseline Intermedia
Console.WriteLine("Interim: {0}", baseline.Interim);
Console.WriteLine("Fixed Cost: {0}", baseline.FixedCost);

// stampa i dati temporizzati della baseline dell'attività
Console.WriteLine("Number of timephased items: " + baseline.TimephasedData.Count);
foreach (var data in baseline.TimephasedData)
{
    Console.WriteLine(" Uid: " + data.Uid);
    Console.WriteLine(" Start: " + data.Start);
    Console.WriteLine(" Finish: " + data.Finish);
}
```

### Vedi anche

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


