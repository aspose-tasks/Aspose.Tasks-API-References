---
title: "Rsc.BudgetCost"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. Costi di budget per le risorse a costo di budget. Le risorse di budget sono assegnate solo all'attività riepilogo del progetto"
type: docs
weight: 170
url: /it/net/aspose.tasks/rsc/budgetcost/
---
## Rsc.BudgetCost field

Costi di budget per le risorse di costo di budget. Le risorse di budget sono assegnate solo all'attività di riepilogo del progetto.

```csharp
public static readonly Key<decimal, RscKey> BudgetCost;
```

## Esempi

Mostra come leggere i valori di lavoro/costo di budget di una risorsa.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

// Visualizza il lavoro di budget e il costo di budget per l'attività riepilogo del progetto
Console.WriteLine("projSummary.BudgetWork = " + project.RootTask.Get(Tsk.BudgetWork));
Console.WriteLine("projSummary.BudgetCost = " + project.RootTask.Get(Tsk.BudgetCost));

// Visualizza il lavoro di budget della risorsa
var rsc = project.Resources.GetByUid(6);
Console.WriteLine("Resource BudgetWork = " + rsc.Get(Rsc.BudgetWork));

// Visualizza il costo di budget della risorsa
rsc = project.Resources.GetByUid(7);
Console.WriteLine("Resource BudgetCost = " + rsc.Get(Rsc.BudgetCost));

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // Visualizza il lavoro di budget e il costo di budget dell'assegnazione
    foreach (var assignment in task.Assignments)
    {
        var resource = assignment.Get(Asn.Resource);
        if (resource == null)
        {
            continue;
        }

        if (resource.Get(Rsc.Type) == ResourceType.Work)
        {
            Console.WriteLine("Assignment BudgetWork = " + assignment.Get(Asn.BudgetWork));
        }
        else
        {
            Console.WriteLine("Assignment BudgetCost = " + assignment.Get(Asn.BudgetCost));
        }
    }
}
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


