---
title: "Task.Equals"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo di Task. Restituisce un valore che indica se questa istanza è uguale a un'attività specificata"
type: docs
weight: 1330
url: /it/net/aspose.tasks/task/equals/
---
## Equals(Task) {#equals}

Restituisce un valore che indica se questa istanza è uguale a un'attività specificata.

```csharp
public bool Equals(Task other)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| altro | Attività | L'attività specificata da confrontare con questa istanza. |

### Valore di ritorno

restituisce true se l'attività specificata e questa istanza hanno ID unici uguali.

## Esempi

Mostra come iterare le assegnazioni dell'attività.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // visualizza le assegnazioni del task
    foreach (var assignment in task.Assignments)
    {
        Console.WriteLine(assignment.ToString());
    }
}
```

### Vedi anche

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato.

```csharp
public override bool Equals(object obj)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | Oggetto | L'oggetto specificato da confrontare con questa istanza. |

### Valore di ritorno

restituisce true se l'attività specificata e questa istanza hanno ID unici uguali.

## Esempi

Mostra come iterare le assegnazioni dell'attività.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // visualizza le assegnazioni del task
    foreach (var assignment in task.Assignments)
    {
        Console.WriteLine(assignment.ToString());
    }
}
```

### Vedi anche

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


