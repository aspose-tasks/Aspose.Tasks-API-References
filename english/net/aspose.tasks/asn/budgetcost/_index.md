---
title: Asn.BudgetCost
second_title: Aspose.Tasks for .NET API Reference
description: Asn field. The budgeted cost of resources on an assignment
type: docs
weight: 150
url: /net/aspose.tasks/asn/budgetcost/
---
## Asn.BudgetCost field

The budgeted cost of resources on an assignment.

```csharp
public static readonly Key<decimal, AsnKey> BudgetCost;
```

## Examples

Shows how to read budget work/cost values of a resource assignment.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

// Display budget work and budget cost for project summary task
Console.WriteLine("projSummary.BudgetWork = " + project.RootTask.Get(Tsk.BudgetWork));
Console.WriteLine("projSummary.BudgetCost = " + project.RootTask.Get(Tsk.BudgetCost));

// Display resource budget work
var rsc = project.Resources.GetByUid(6);
Console.WriteLine("Resource BudgetWork = " + rsc.Get(Rsc.BudgetWork));

// Display resource budget cost
rsc = project.Resources.GetByUid(7);
Console.WriteLine("Resource BudgetCost = " + rsc.Get(Rsc.BudgetCost));

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var tsk in collector.Tasks)
{
    // Display assignment budget work and budget cost
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

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


