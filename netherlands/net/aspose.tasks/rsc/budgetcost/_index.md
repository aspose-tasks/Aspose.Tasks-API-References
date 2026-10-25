---
title: "Rsc.BudgetCost"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc-veld. Budgetkosten voor budgetkost-resources. Budgetresources worden alleen toegewezen aan de projectoverzichtstaak."
type: docs
weight: 170
url: /nl/net/aspose.tasks/rsc/budgetcost/
---
## Rsc.BudgetCost field

Begrote kosten voor budgetkostresources. Budgetkostresources worden alleen toegewezen aan de projectoverzichtstaak.

```csharp
public static readonly Key<decimal, RscKey> BudgetCost;
```

## Voorbeelden

Toont hoe de budgetwerk-/kostwaarden van een resource gelezen kunnen worden.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

// Toon budgetwerk en budgetkosten voor de samenvattende taak van het project
Console.WriteLine("projSummary.BudgetWork = " + project.RootTask.Get(Tsk.BudgetWork));
Console.WriteLine("projSummary.BudgetCost = " + project.RootTask.Get(Tsk.BudgetCost));

// Toon resourcebudgetwerk
var rsc = project.Resources.GetByUid(6);
Console.WriteLine("Resource BudgetWork = " + rsc.Get(Rsc.BudgetWork));

// Toon resourcebudgetkosten
rsc = project.Resources.GetByUid(7);
Console.WriteLine("Resource BudgetCost = " + rsc.Get(Rsc.BudgetCost));

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // Toon toewijzingsbudgetwerk en budgetkosten
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

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


