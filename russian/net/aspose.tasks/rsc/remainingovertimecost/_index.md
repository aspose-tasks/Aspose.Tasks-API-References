---
title: "Rsc.RemainingOvertimeCost"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Оставшиеся запланированные расходы на сверхурочную работу для ресурса"
type: docs
weight: 590
url: /ru/net/aspose.tasks/rsc/remainingovertimecost/
---
## Rsc.RemainingOvertimeCost field

Оставшиеся запланированные расходы на сверхурочную работу для ресурса.

```csharp
public static readonly Key<decimal, RscKey> RemainingOvertimeCost;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.RemainingOvertimeCost.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingOvertimeCost, 3);

Console.WriteLine("Remaining Overtime Cost: " + resource.Get(Rsc.RemainingOvertimeCost));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


