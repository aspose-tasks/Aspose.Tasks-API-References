---
title: "Asn.WorkVariance"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Asn. Разница между базовой работой задачи и текущей запланированной работой"
type: docs
weight: 620
url: /ru/net/aspose.tasks/asn/workvariance/
---
## Asn.WorkVariance field

Разница между базовой работой задачи и текущей запланированной работой.

```csharp
public static readonly Key<Duration, AsnKey> WorkVariance;
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


