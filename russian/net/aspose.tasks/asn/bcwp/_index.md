---
title: "Asn.BCWP"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Asn. Запланированная стоимость выполненной работы в назначении на текущую дату"
type: docs
weight: 120
url: /ru/net/aspose.tasks/asn/bcwp/
---
## Asn.BCWP field

Запланированная стоимость выполненной работы по назначению на текущую дату.

```csharp
public static readonly Key<double, AsnKey> BCWP;
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


