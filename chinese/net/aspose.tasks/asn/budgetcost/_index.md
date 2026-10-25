---
title: "Asn.BudgetCost"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Asn 字段。分配中资源的预算成本"
type: docs
weight: 150
url: /zh/net/aspose.tasks/asn/budgetcost/
---
## Asn.BudgetCost field

任务中资源的预算成本。

```csharp
public static readonly Key<decimal, AsnKey> BudgetCost;
```

## 示例

展示如何读取资源任务的预算工作/成本值。

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

// 显示项目汇总任务的预算工作和预算成本.
Console.WriteLine("projSummary.BudgetWork = " + project.RootTask.Get(Tsk.BudgetWork));
Console.WriteLine("projSummary.BudgetCost = " + project.RootTask.Get(Tsk.BudgetCost));

// 显示资源预算工作.
var rsc = project.Resources.GetByUid(6);
Console.WriteLine("Resource BudgetWork = " + rsc.Get(Rsc.BudgetWork));

// 显示资源预算成本.
rsc = project.Resources.GetByUid(7);
Console.WriteLine("Resource BudgetCost = " + rsc.Get(Rsc.BudgetCost));

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var tsk in collector.Tasks)
{
    // 显示分配的预算工作和预算成本.
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

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


