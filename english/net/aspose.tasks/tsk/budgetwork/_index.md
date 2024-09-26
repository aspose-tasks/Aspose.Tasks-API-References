---
title: Tsk.BudgetWork
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. Budget work for budget work and material resources. Budget resources are assigned only to the project summary task
type: docs
weight: 150
url: /net/aspose.tasks/tsk/budgetwork/
---
## Tsk.BudgetWork field

Budget work for budget work and material resources. Budget resources are assigned only to the project summary task.

```csharp
public static readonly Key<Duration, TaskKey> BudgetWork;
```

## Examples

Shows how to read budget work/cost values of task/resource/assignment.

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
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


