---
title: "Tsk.BudgetCost"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Бюджетные затраты для ресурсов с бюджетными расходами. Бюджетные ресурсы назначаются только задаче‑сводке проекта"
type: docs
weight: 140
url: /ru/net/aspose.tasks/tsk/budgetcost/
---
## Tsk.BudgetCost field

Бюджетные затраты для ресурсов с бюджетными затратами. Бюджетные ресурсы назначаются только задаче‑сводке проекта.

```csharp
public static readonly Key<decimal, TaskKey> BudgetCost;
```

## Примеры

Показывает, как читать значения бюджетной работы/стоимости задачи/ресурса/назначения.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

// Отобразить бюджетные трудозатраты и бюджетную стоимость для задачи сводки проекта
Console.WriteLine("projSummary.BudgetWork = " + project.RootTask.Get(Tsk.BudgetWork));
Console.WriteLine("projSummary.BudgetCost = " + project.RootTask.Get(Tsk.BudgetCost));

// Отобразить бюджетные трудозатраты ресурса
var rsc = project.Resources.GetByUid(6);
Console.WriteLine("Resource BudgetWork = " + rsc.Get(Rsc.BudgetWork));

// Отобразить бюджетную стоимость ресурса
rsc = project.Resources.GetByUid(7);
Console.WriteLine("Resource BudgetCost = " + rsc.Get(Rsc.BudgetCost));

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var tsk in collector.Tasks)
{
    // Отобразить бюджетные трудозатраты и бюджетную стоимость назначения
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

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


