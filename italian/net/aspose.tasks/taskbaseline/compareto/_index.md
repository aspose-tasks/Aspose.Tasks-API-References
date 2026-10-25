---
title: "TaskBaseline.CompareTo"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo TaskBaseline. Implementazione dell'interfaccia IComparable. Confronta questa istanza con l'oggetto Baseline specificato"
type: docs
weight: 90
url: /it/net/aspose.tasks/taskbaseline/compareto/
---
## TaskBaseline.CompareTo method

Implementazione dell'interfaccia IComparable. Confronta questa istanza con l'oggetto Baseline specificato.

```csharp
public int CompareTo(TaskBaseline other)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| altro | TaskBaseline | l'oggetto Baseline specificato con cui confrontare questa istanza. |

### Valore di ritorno

restituisce -1 se questa istanza è inferiore all'oggetto specificato, 1 se questa istanza è superiore all'oggetto specificato; altrimenti restituisce 0

## Esempi

Mostra come verificare l'uguaglianza delle baseline.

```csharp
var project = new Project();

// creazione di TaskBaseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// visualizza la durata della baseline dell'attività
var baseline1 = task.Baselines.ToList()[0];
var baseline2 = task.Baselines.ToList()[0];

// l'uguaglianza delle baseline è verificata confrontando i numeri delle baseline.
Console.WriteLine("Baseline Number 1: " + baseline1.BaselineNumber);
Console.WriteLine("Baseline Number 2: " + baseline2.BaselineNumber);
Console.WriteLine("Are baselines equal: " + baseline1.Equals(baseline2));
```

### Vedi anche

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


