---
title: "ResourceAssignment.ToString"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ResourceAssignment. Restituisce una breve rappresentazione stringa dell'istanza della classe ResourceAssignment. I dettagli esatti della rappresentazione non sono specificati e sono soggetti a modifiche"
type: docs
weight: 790
url: /it/net/aspose.tasks/resourceassignment/tostring/
---
## ResourceAssignment.ToString method

Restituisce una breve rappresentazione stringa dell'istanza della classe [`ResourceAssignment`](../). I dettagli esatti della rappresentazione non sono specificati e sono soggetti a modifiche.

```csharp
public override string ToString()
```

### Valore di ritorno

breve stringa che rappresenta l'oggetto di assegnazione.

## Esempi

Mostra come stampare le informazioni comuni di assegnazione.

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

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


