---
title: "Rsc.AvailableFrom"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Начальная дата, с которой ресурс доступен для работы в указанных единицах текущего периода"
type: docs
weight: 120
url: /ru/net/aspose.tasks/rsc/availablefrom/
---
## Rsc.AvailableFrom field

Дата начала, с которой ресурс доступен для работы в указанных единицах за текущий период.

```csharp
public static readonly Key<DateTime, RscKey> AvailableFrom;
```

## Примеры

Показывает, как прочитать/записать свойство Rsc.AvailableFrom.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AvailableFrom, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Available From: " + resource.Get(Rsc.AvailableFrom));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


