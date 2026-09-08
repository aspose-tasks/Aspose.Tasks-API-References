---
title: "Rsc.WorkVariance"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Разница между базовой работой ресурса и текущей запланированной работой"
type: docs
weight: 710
url: /ru/net/aspose.tasks/rsc/workvariance/
---
## Rsc.WorkVariance field

Разница между базовой работой ресурса и текущей запланированной работой.

```csharp
public static readonly Key<double, RscKey> WorkVariance;
```

## Примеры

Показывает, как читать отклонение работы ресурса.

```csharp
var project = new Project(DataDir + "WorkVariance.mpp");

foreach (var assignment in project.ResourceAssignments)
{
    var resource = assignment.Get(Asn.Resource);

    var workVariance = resource.Get(Rsc.WorkVariance);

    Console.WriteLine(workVariance);
}
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


