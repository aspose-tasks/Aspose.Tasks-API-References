---
title: "Classe TaskBaseline"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.TaskBaseline. Rappresenta la baseline di un Task"
type: docs
weight: 2370
url: /it/net/aspose.tasks/taskbaseline/
---
## TaskBaseline class

Rappresenta la baseline di un'attività.

```csharp
public sealed class TaskBaseline : Baseline, IComparable<TaskBaseline>, IEquatable<TaskBaseline>
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [TaskBaseline](taskbaseline/)(Task) | Inizializza una nuova istanza della classe `TaskBaseline`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BaselineNumber](../../aspose.tasks/baseline/baselinenumber/) { get; set; } | Ottiene o imposta il numero univoco di un record di dati di baseline. |
| [Bcwp](../../aspose.tasks/baseline/bcwp/) { get; set; } | Ottiene o imposta il costo preventivato di un lavoro eseguito da una risorsa per un progetto fino ad oggi. |
| [Bcws](../../aspose.tasks/baseline/bcws/) { get; set; } | Ottiene o imposta il costo preventivo di un lavoro programmato per una risorsa. |
| [Cost](../../aspose.tasks/baseline/cost/) { get; set; } | Ottiene o imposta il costo previsto di una risorsa quando la baseline viene salvata. |
| [Duration](../../aspose.tasks/taskbaseline/duration/) { get; set; } | Ottiene o imposta la durata programmata dell'attività quando è stata salvata la baseline. |
| [EstimatedDuration](../../aspose.tasks/taskbaseline/estimatedduration/) { get; set; } | Ottiene o imposta un valore che indica se la durata della baseline dell'attività è stata stimata. |
| [Finish](../../aspose.tasks/taskbaseline/finish/) { get; set; } | Ottiene o imposta la data di fine programmata dell'attività quando è stata salvata la baseline. |
| [FixedCost](../../aspose.tasks/taskbaseline/fixedcost/) { get; set; } | Ottiene o imposta un costo fisso dell'attività quando è stata salvata la baseline. |
| [Interim](../../aspose.tasks/taskbaseline/interim/) { get; set; } | Ottiene o imposta un valore che indica se questa è una Baseline Intermedia. |
| [Start](../../aspose.tasks/taskbaseline/start/) { get; set; } | Ottiene o imposta la data di inizio programmata dell'attività quando è stata salvata la baseline. |
| [TimephasedData](../../aspose.tasks/taskbaseline/timephaseddata/) { get; set; } | Ottiene o imposta un'istanza di TimephasedDataCollection per questo oggetto. I dati temporizzati associati alla baseline dell'attività. |
| [Work](../../aspose.tasks/baseline/work/) { get; set; } | Ottiene o imposta il lavoro assegnato a una risorsa quando la baseline è salvata. La quantità di lavoro assegnato a una risorsa quando la baseline è stata salvata. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [CompareTo](../../aspose.tasks/baseline/compareto/)(Baseline) | Implementazione dell'interfaccia IComparable. Confronta questa istanza con l'oggetto Baseline specificato. |
| [CompareTo](../../aspose.tasks/taskbaseline/compareto/#compareto_1)(TaskBaseline) | Implementazione dell'interfaccia IComparable. Confronta questa istanza con l'oggetto Baseline specificato. |
| [Equals](../../aspose.tasks/baseline/equals/)(Baseline) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| override [Equals](../../aspose.tasks/taskbaseline/equals/#equals_2)(object) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| [Equals](../../aspose.tasks/taskbaseline/equals/#equals_1)(TaskBaseline) | Restituisce un valore che indica se questa istanza è uguale all'oggetto TaskBaseline specificato. |
| override [GetHashCode](../../aspose.tasks/taskbaseline/gethashcode/)() | Restituisce un valore di codice hash per l'istanza della classe `TaskBaseline`. |

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

* class [Baseline](../baseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


