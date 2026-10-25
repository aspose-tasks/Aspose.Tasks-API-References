---
title: "Asn.CostVariance"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Asn. Разница между базовой стоимостью и общей стоимостью назначения"
type: docs
weight: 200
url: /ru/net/aspose.tasks/asn/costvariance/
---
## Asn.CostVariance field

Разница между базовой стоимостью и общей стоимостью назначения.

```csharp
public static readonly Key<double, AsnKey> CostVariance;
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
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


