---
title: "TaskBaseline.GetHashCode"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo TaskBaseline. Restituisce un valore di codice hash per l'istanza della classe TaskBaseline"
type: docs
weight: 110
url: /it/net/aspose.tasks/taskbaseline/gethashcode/
---
## TaskBaseline.GetHashCode method

Restituisce un valore di codice hash per l'istanza della classe [`TaskBaseline`](../).

```csharp
public override int GetHashCode()
```

### Valore di ritorno

restituisce un valore di hash per questo oggetto.

## Esempi

Mostra come ottenere il codice hash di un baseline di attività.

```csharp
var project = new Project();

// creazione di TaskBaseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// visualizza la durata della baseline dell'attività
var baseline1 = task.Baselines.ToList()[0];
var baseline2 = task.Baselines.ToList()[0];

// Il codice hash di un calendario è uguale al numero del baseline 
Console.WriteLine("Baseline 1 Number: {0} Hash Code: {1}", (int)baseline1.BaselineNumber, baseline1.GetHashCode());
Console.WriteLine("Baseline 2 Number: {0} Hash Code: {1}", (int)baseline2.BaselineNumber, baseline2.GetHashCode());
```

### Vedi anche

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


