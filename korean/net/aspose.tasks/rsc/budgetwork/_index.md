---
title: "Rsc.BudgetWork"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 예산 작업은 예산 작업 및 물자 자원에 대한 것입니다. 예산 자원은 프로젝트 요약 작업에만 할당됩니다."
type: docs
weight: 180
url: /ko/net/aspose.tasks/rsc/budgetwork/
---
## Rsc.BudgetWork field

예산 작업 및 자재 리소스에 대한 예산 작업. 예산 리소스는 프로젝트 요약 작업에만 할당됩니다.

```csharp
public static readonly Key<Duration, RscKey> BudgetWork;
```

## 예제

리소스의 예산 작업/비용 값을 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

// 프로젝트 요약 작업에 대한 예산 작업 및 예산 비용을 표시합니다.
Console.WriteLine("projSummary.BudgetWork = " + project.RootTask.Get(Tsk.BudgetWork));
Console.WriteLine("projSummary.BudgetCost = " + project.RootTask.Get(Tsk.BudgetCost));

// 리소스 예산 작업을 표시합니다.
var rsc = project.Resources.GetByUid(6);
Console.WriteLine("Resource BudgetWork = " + rsc.Get(Rsc.BudgetWork));

// 리소스 예산 비용을 표시합니다.
rsc = project.Resources.GetByUid(7);
Console.WriteLine("Resource BudgetCost = " + rsc.Get(Rsc.BudgetCost));

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // 할당 예산 작업 및 예산 비용을 표시합니다.
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

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


