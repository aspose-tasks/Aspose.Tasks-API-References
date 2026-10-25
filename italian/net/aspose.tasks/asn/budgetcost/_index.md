---
title: "Asn.BudgetCost"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Asn. Il costo preventivato delle risorse su un'assegnazione"
type: docs
weight: 150
url: /it/net/aspose.tasks/asn/budgetcost/
---
## Asn.BudgetCost field

Il costo preventivato delle risorse su un'assegnazione.

```csharp
public static readonly Key<decimal, AsnKey> BudgetCost;
```

## Esempi

Mostra come leggere i valori di lavoro/costo preventivo di un'assegnazione di risorsa.

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
foreach (var tsk in collector.Tasks)
{
    // Visualizza il lavoro di budget e il costo di budget dell'assegnazione
    foreach (var assignment in tsk.Assignments)
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
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


