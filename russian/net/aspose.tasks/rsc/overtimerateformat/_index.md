---
title: "Rsc.OvertimeRateFormat"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Единицы, используемые Microsoft Project для отображения ставки сверхурочных"
type: docs
weight: 520
url: /ru/net/aspose.tasks/rsc/overtimerateformat/
---
## Rsc.OvertimeRateFormat field

Единицы, используемые Microsoft Project для отображения ставки сверхурочных.

```csharp
public static readonly Key<RateFormatType, RscKey> OvertimeRateFormat;
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
* enum [RateFormatType](../../rateformattype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


