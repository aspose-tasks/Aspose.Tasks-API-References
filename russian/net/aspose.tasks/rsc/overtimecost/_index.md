---
title: "Rsc.OvertimeCost"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Rsc field. Общая стоимость сверхурочной работы ресурса по всем назначенным задачам"
type: docs
weight: 500
url: /ru/net/aspose.tasks/rsc/overtimecost/
---
## Rsc.OvertimeCost field

Общая стоимость сверхурочных для ресурса по всем назначенным задачам.

```csharp
public static readonly Key<decimal, RscKey> OvertimeCost;
```

## Примеры

Показывает, как читать значения сверхурочной работы ресурса.

```csharp
var project = new Project(DataDir + "ResourceOvertime.mpp");

// Отображать параметры, связанные со сверхурочной работой, для всех ресурсов
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) == null)
    {
        continue;
    }

    Console.WriteLine(res.Get(Rsc.OvertimeCost));
    Console.WriteLine(res.Get(Rsc.OvertimeWork).ToString());
    Console.WriteLine(res.Get(Rsc.OvertimeRateFormat).ToString());
}
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


