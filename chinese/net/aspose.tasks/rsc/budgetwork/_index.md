---
title: "Rsc.BudgetWork"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段. 预算工作用于预算工作和材料资源. 预算资源仅分配给项目汇总任务."
type: docs
weight: 180
url: /zh/net/aspose.tasks/rsc/budgetwork/
---
## Rsc.BudgetWork field

预算工作用于预算工作和材料资源。预算资源仅分配给项目汇总任务。

```csharp
public static readonly Key<Duration, RscKey> BudgetWork;
```

## 示例

展示如何读取资源的预算工作/成本值.

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
foreach (var task in collector.Tasks)
{
    // 显示分配的预算工作和预算成本.
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

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


