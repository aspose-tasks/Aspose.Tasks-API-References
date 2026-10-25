---
title: "Asn.SV"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Asn. Отклонение графика заработанной стоимости на дату статуса проекта. Отклонение графика SV — это разница между BCWP и BCWS"
type: docs
weight: 540
url: /ru/net/aspose.tasks/asn/sv/
---
## Asn.SV field

Отклонение графика заработанной стоимости на текущую дату статуса. Отклонение графика (SV) — это разница между BCWP и BCWS.

```csharp
public static readonly Key<double, AsnKey> SV;
```

## Примеры

Показывает, как читать значения стоимости назначения.

```csharp
var project = new Project(DataDir + "ResourceAssignmentCosts.mpp");

// Печать стоимостей назначения ресурса
foreach (var assignment in project.ResourceAssignments)
{
    Console.WriteLine(assignment.Get(Asn.Cost));
    Console.WriteLine(assignment.Get(Asn.ACWP));

    // CV = BCWP - ACWP
    Console.WriteLine(assignment.Get(Asn.CV));

    Console.WriteLine(assignment.Get(Asn.BCWP));
    Console.WriteLine(assignment.Get(Asn.BCWS));

    // SV = BCWP - BCWS
    Console.WriteLine(assignment.Get(Asn.SV));
}
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


