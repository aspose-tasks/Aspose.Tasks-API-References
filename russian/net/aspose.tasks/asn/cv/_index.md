---
title: "Asn.CV"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Asn. Отклонение стоимости заработанной стоимости. CV — это разница между плановой стоимостью выполненных работ (BCWP) и фактической стоимостью выполненных работ (ACWP) для назначения."
type: docs
weight: 220
url: /ru/net/aspose.tasks/asn/cv/
---
## Asn.CV field

Отклонение стоимости заработанной стоимости. CV — это разница между BCWP (запланированная стоимость выполненной работы) и ACWP (фактическая стоимость выполненной работы) назначения.

```csharp
public static readonly Key<double, AsnKey> CV;
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


