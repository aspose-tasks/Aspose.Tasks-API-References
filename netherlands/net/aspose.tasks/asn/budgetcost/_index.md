---
title: "Asn.BudgetCost"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Asn-veld. De begrote kosten van resources op een toewijzing"
type: docs
weight: 150
url: /nl/net/aspose.tasks/asn/budgetcost/
---
## Asn.BudgetCost field

De begrote kosten van middelen op een opdracht.

```csharp
public static readonly Key<decimal, AsnKey> BudgetCost;
```

## Voorbeelden

Toont hoe de budgetwerk-/kostwaarden van een resource-toewijzing gelezen kunnen worden.

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
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


