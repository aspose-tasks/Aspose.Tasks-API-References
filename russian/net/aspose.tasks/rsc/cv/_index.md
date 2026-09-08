---
title: "Rsc.CV"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Отклонение стоимости заработанной стоимости к дате статуса проекта. CV — это разница между запланированной стоимостью выполненной работы (BCWP) задачи и фактической стоимостью выполненной работы (ACWP)."
type: docs
weight: 270
url: /ru/net/aspose.tasks/rsc/cv/
---
## Rsc.CV field

Отклонение стоимости заработанной стоимости до даты статуса проекта. CV — это разница между BCWP (бюджетная стоимость выполненной работы) задачи и ACWP (фактическая стоимость выполненной работы).

```csharp
public static readonly Key<double, RscKey> CV;
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


