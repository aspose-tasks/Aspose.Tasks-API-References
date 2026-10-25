---
title: "Rsc.Cost"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Общая запланированная или прогнозируемая стоимость ресурса, основанная на уже понесённых расходах за работу, выполненную ресурсами, назначенными на задачи, а также на расходах, запланированных для оставшейся работы"
type: docs
weight: 220
url: /ru/net/aspose.tasks/rsc/cost/
---
## Rsc.Cost field

Общая запланированная или прогнозируемая стоимость ресурса, основанная на уже понесённых затратах за выполненную ресурсами работу, а также на планируемых затратах на оставшуюся работу.

```csharp
public static readonly Key<decimal, RscKey> Cost;
```

## Примеры

Показывает, как читать затраты ресурса.

```csharp
var project = new Project(DataDir + "ResourceCosts.mpp");

// Отобразить все затраты ресурсов
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) == null)
    {
        continue;
    }

    Console.WriteLine(res.Get(Rsc.Cost));
    Console.WriteLine(res.Get(Rsc.ACWP));
    Console.WriteLine(res.Get(Rsc.BCWS));
    Console.WriteLine(res.Get(Rsc.BCWP));

    // CV = BCWP - ACWP
    Console.WriteLine(res.Get(Rsc.CV));

    // SV = BCWP - BCWS
    Console.WriteLine(res.Get(Rsc.SV));
}
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


