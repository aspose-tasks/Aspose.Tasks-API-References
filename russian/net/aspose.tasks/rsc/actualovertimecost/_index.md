---
title: "Rsc.ActualOvertimeCost"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Rsc field. Затраты, понесённые за сверхурочную работу, уже выполненную над задачами назначенными ресурсами"
type: docs
weight: 40
url: /ru/net/aspose.tasks/rsc/actualovertimecost/
---
## Rsc.ActualOvertimeCost field

Затраты, возникшие в результате уже выполненной сверхурочной работы над задачами назначенными ресурсами.

```csharp
public static readonly Key<decimal, RscKey> ActualOvertimeCost;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.ActualOvertimeCost.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeCost, 10m);

Console.WriteLine("Actual Overtime Cost: " + resource.Get(Rsc.ActualOvertimeCost));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


