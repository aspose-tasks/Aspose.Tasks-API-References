---
title: "Rsc.ActualCost"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Затраты, понесённые за уже выполненную ресурсами работу над их задачами, а также любые другие зарегистрированные затраты, связанные с задачей"
type: docs
weight: 30
url: /ru/net/aspose.tasks/rsc/actualcost/
---
## Rsc.ActualCost field

Затраты, возникшие в результате уже выполненной ресурсов работы над их задачами, а также любые другие зарегистрированные затраты, связанные с задачей.

```csharp
public static readonly Key<decimal, RscKey> ActualCost;
```

## Примеры

Показывает, как прочитать/записать свойство Rsc.ActualCost.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualCost, 10m);

Console.WriteLine("Actual Cost: " + resource.Get(Rsc.ActualCost));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


