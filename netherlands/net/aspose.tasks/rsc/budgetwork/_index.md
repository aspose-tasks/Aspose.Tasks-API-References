---
title: "Rsc.BudgetWork"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc-veld. budgetwerk voor budgetwerk en materiële middelen. Budgetmiddelen worden alleen toegewezen aan de samenvattende taak van het project"
type: docs
weight: 180
url: /nl/net/aspose.tasks/rsc/budgetwork/
---
## Rsc.BudgetWork field

Begroot werk voor budgetwerk- en materiaalsresources. Budgetresources worden alleen toegewezen aan de projectoverzichtstaak.

```csharp
public static readonly Key<Duration, RscKey> BudgetWork;
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
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


