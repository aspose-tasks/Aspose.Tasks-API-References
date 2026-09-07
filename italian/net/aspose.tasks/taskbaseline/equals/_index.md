---
title: "TaskBaseline.Equals"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo TaskBaseline. Restituisce un valore che indica se questa istanza è uguale all'oggetto TaskBaseline specificato"
type: docs
weight: 100
url: /it/net/aspose.tasks/taskbaseline/equals/
---
## Equals(TaskBaseline) {#equals_1}

Restituisce un valore che indica se questa istanza è uguale all'oggetto TaskBaseline specificato.

```csharp
public bool Equals(TaskBaseline other)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| altro | TaskBaseline | l'oggetto AssignmentBaseline specificato da confrontare con questa istanza. |

### Valore di ritorno

Restituisce true se questa istanza è uguale all'oggetto TaskBaseline specificato; altrimenti, false.

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

---

## Equals(object) {#equals_2}

Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato.

```csharp
public override bool Equals(object obj)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | Oggetto | L'oggetto da confrontare con questa istanza. |

### Valore di ritorno

**True** if the specified object is a TaskBaseline that has the same UID value as this instance; otherwise, **false**.

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


