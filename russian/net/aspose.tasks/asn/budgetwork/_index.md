---
title: "Asn.BudgetWork"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Asn. Запланированное количество работы для трудовых или материальных ресурсов в назначении"
type: docs
weight: 160
url: /ru/net/aspose.tasks/asn/budgetwork/
---
## Asn.BudgetWork field

Запланированное количество работы для трудовых или материальных ресурсов по назначению.

```csharp
public static readonly Key<Duration, AsnKey> BudgetWork;
```

## Примеры

Показывает, как считывать значения запланированных работы/стоимости ресурса в назначении.

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
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


