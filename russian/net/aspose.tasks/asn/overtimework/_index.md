---
title: "Asn.OvertimeWork"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Asn. Запланированная сверхурочная работа назначения"
type: docs
weight: 380
url: /ru/net/aspose.tasks/asn/overtimework/
---
## Asn.OvertimeWork field

Запланированная сверхурочная работа по назначению.

```csharp
public static readonly Key<Duration, AsnKey> OvertimeWork;
```

## Примеры

Показывает, как читать сверхурочные/оставшиеся работы/затраты задания.

```csharp
var project = new Project(DataDir + "ResourceAssignmentOvertimes.mpp");

// Печать сверхурочных заданий
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.OvertimeWork).ToString());
    Console.WriteLine(ra.Get(Asn.OvertimeCost));
    Console.WriteLine(ra.Get(Asn.RemainingWork).ToString());
    Console.WriteLine(ra.Get(Asn.RemainingCost));
    Console.WriteLine(ra.Get(Asn.RemainingOvertimeWork).ToString());
    Console.WriteLine(ra.Get(Asn.RemainingOvertimeCost));
}
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


