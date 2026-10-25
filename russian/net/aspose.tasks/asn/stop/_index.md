---
title: "Asn.Stop"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Asn. Дата, когда назначение остановлено"
type: docs
weight: 520
url: /ru/net/aspose.tasks/asn/stop/
---
## Asn.Stop field

Дата остановки назначения.

```csharp
public static readonly Key<DateTime, AsnKey> Stop;
```

## Примеры

Показывает, как читать даты остановки/возобновления назначения.

```csharp
var project = new Project(DataDir + "ResourceAssignmentStopResumeDates.mpp");

// Печать дат остановки и возобновления назначения ресурса
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.Stop).ToShortDateString() == "1/1/2000" ? "NA" : ra.Get(Asn.Stop).ToShortDateString());
    Console.WriteLine(ra.Get(Asn.Resume).ToShortDateString() == "1/1/2000" ? "NA" : ra.Get(Asn.Resume).ToShortDateString());
}
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


