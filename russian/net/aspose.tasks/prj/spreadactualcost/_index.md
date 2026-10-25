---
title: "Prj.SpreadActualCost"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Определяет, распространяются ли фактические затраты на дату статуса"
type: docs
weight: 660
url: /ru/net/aspose.tasks/prj/spreadactualcost/
---
## Prj.SpreadActualCost field

Определяет, распределяются ли фактические затраты по дате статуса.

```csharp
public static readonly Key<NullableBool, PrjKey> SpreadActualCost;
```

## Примеры

Показывает, как читать/записывать свойство Prj.SpreadActualCost.

```csharp
var project = new Project();

project.Set(Prj.SpreadActualCost, true);

Console.WriteLine("Spread Actual Cost: " + project.Get(Prj.SpreadActualCost));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


