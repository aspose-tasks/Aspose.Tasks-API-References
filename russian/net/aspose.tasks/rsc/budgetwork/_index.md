---
title: "Rsc.BudgetWork"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. рабочие часы бюджета для бюджетных и материальных ресурсов. Бюджетные ресурсы назначаются только задаче сводки проекта"
type: docs
weight: 180
url: /ru/net/aspose.tasks/rsc/budgetwork/
---
## Rsc.BudgetWork field

Бюджетная работа для бюджетных и материальных ресурсов. Бюджетные ресурсы назначаются только задаче‑сводке проекта.

```csharp
public static readonly Key<Duration, RscKey> BudgetWork;
```

## Примеры

Показывает, как прочитать значения бюджетных трудозатрат/стоимости ресурса.

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
foreach (var task in collector.Tasks)
{
    // Отобразить бюджетные трудозатраты и бюджетную стоимость назначения
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

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


