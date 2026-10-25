---
title: "Asn.StartVariance"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Asn. Отклонение даты начала назначения от базовой даты начала"
type: docs
weight: 510
url: /ru/net/aspose.tasks/asn/startvariance/
---
## Asn.StartVariance field

Отклонение даты начала назначения от базовой даты начала.

```csharp
public static readonly Key<Duration, AsnKey> StartVariance;
```

## Примеры

Показывает, как читать отклонения назначения.

```csharp
var project = new Project(DataDir + "ResourceAssignmentVariance.mpp");

// Печать отклонений назначения
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.WorkVariance));
    Console.WriteLine(ra.Get(Asn.CostVariance));
    Console.WriteLine(ra.Get(Asn.StartVariance));
    Console.WriteLine(ra.Get(Asn.FinishVariance));
}
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


