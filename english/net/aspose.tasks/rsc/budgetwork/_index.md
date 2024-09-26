---
title: Rsc.BudgetWork
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. budget work for budget work and material resources. Budget resources are assigned only to the project summary task
type: docs
weight: 180
url: /net/aspose.tasks/rsc/budgetwork/
---
## Rsc.BudgetWork field

budget work for budget work and material resources. Budget resources are assigned only to the project summary task.

```csharp
public static readonly Key<Duration, RscKey> BudgetWork;
```

## Examples

Shows how to read budget work/cost values of a resource.

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
foreach (var task in collector.Tasks)
{
    // Display assignment budget work and budget cost
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

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


