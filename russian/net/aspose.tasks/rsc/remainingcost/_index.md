---
title: "Rsc.RemainingCost"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Оставшиеся запланированные расходы, которые будут понесены при завершении оставшейся запланированной работы"
type: docs
weight: 580
url: /ru/net/aspose.tasks/rsc/remainingcost/
---
## Rsc.RemainingCost field

Оставшиеся запланированные расходы, которые будут понесены при выполнении оставшейся запланированной работы.

```csharp
public static readonly Key<decimal, RscKey> RemainingCost;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.RemainingCost.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingCost, 2);

Console.WriteLine("Remaining Cost: " + resource.Get(Rsc.RemainingCost));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


