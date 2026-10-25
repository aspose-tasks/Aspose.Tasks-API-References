---
title: "Tsk.BudgetCost"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. Budgetkosten voor budgetkostbronnen. Budgetbronnen worden alleen toegewezen aan de project‑samenvattingstaak."
type: docs
weight: 140
url: /nl/net/aspose.tasks/tsk/budgetcost/
---
## Tsk.BudgetCost field

Begrote kosten voor budgetkostresources. Budgetkostresources worden alleen toegewezen aan de projectoverzichtstaak.

```csharp
public static readonly Key<decimal, TaskKey> BudgetCost;
```

## Voorbeelden

Toont hoe budgetwerk-/kostwaarden van taak/resource/toewijzing gelezen kunnen worden.

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
foreach (var tsk in collector.Tasks)
{
    // Toon toewijzingsbudgetwerk en budgetkosten
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

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


