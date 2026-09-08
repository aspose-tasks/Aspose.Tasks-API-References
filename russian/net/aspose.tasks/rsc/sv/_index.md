---
title: "Rsc.SV"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Отклонение графика заработанной стоимости на дату статуса проекта. SV — это разница между запланированной стоимостью выполненной работы (BCWP) и запланированной стоимостью запланированной работы (BCWS)."
type: docs
weight: 650
url: /ru/net/aspose.tasks/rsc/sv/
---
## Rsc.SV field

Отклонение графика заработанной стоимости на дату статуса проекта. SV — это разница между запланированной стоимостью выполненной работы (BCWP) и запланированной стоимостью запланированной работы (BCWS).

```csharp
public static readonly Key<double, RscKey> SV;
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


