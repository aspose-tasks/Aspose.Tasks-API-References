---
title: "Asn.ACWP"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Asn. Фактическая стоимость выполненной работы по назначению на текущую дату"
type: docs
weight: 90
url: /ru/net/aspose.tasks/asn/acwp/
---
## Asn.ACWP field

Фактическая стоимость выполненной работы по назначению на текущую дату.

```csharp
public static readonly Key<double, AsnKey> ACWP;
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


