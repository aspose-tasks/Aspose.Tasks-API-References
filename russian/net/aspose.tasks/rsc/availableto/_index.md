---
title: "Rsc.AvailableTo"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Конечная дата, до которой ресурс доступен для работы в указанных единицах текущего периода"
type: docs
weight: 130
url: /ru/net/aspose.tasks/rsc/availableto/
---
## Rsc.AvailableTo field

Дата окончания, до которой ресурс доступен для работы в указанных единицах за текущий период.

```csharp
public static readonly Key<DateTime, RscKey> AvailableTo;
```

## Примеры

Показывает, как прочитать/записать свойство Rsc.AvailableTo.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AvailableTo, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Available To: " + resource.Get(Rsc.AvailableTo));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


