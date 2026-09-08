---
title: "Asn.PercentWorkComplete"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Asn. Объём выполненной работы по назначению"
type: docs
weight: 400
url: /ru/net/aspose.tasks/asn/percentworkcomplete/
---
## Asn.PercentWorkComplete field

Объём выполненной работы по назначению.

```csharp
public static readonly Key<int, AsnKey> PercentWorkComplete;
```

## Примеры

Показывает, как читать процент завершённой работы по назначению.

```csharp
var project = new Project(DataDir + "ResourceAssignmentPercentWorkComplete.mpp");

// Печать процента завершения назначения
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.PercentWorkComplete).ToString());
}
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


