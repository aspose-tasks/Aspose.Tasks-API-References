---
title: "Rsc.OvertimeWork"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Количество сверхурочной работы, запланированной для выполнения ресурсом в задаче и оплачиваемой по сверхурочным ставкам задействованных ресурсов"
type: docs
weight: 530
url: /ru/net/aspose.tasks/rsc/overtimework/
---
## Rsc.OvertimeWork field

Объём сверхурочных, запланированных для выполнения ресурсом в задаче и начисляемых по ставкам сверхурочных задействованных ресурсов.

```csharp
public static readonly Key<Duration, RscKey> OvertimeWork;
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
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


