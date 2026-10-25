---
title: "Rsc.Start"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Дата, когда назначенный ресурс планируется начать работу над задачей."
type: docs
weight: 640
url: /ru/net/aspose.tasks/rsc/start/
---
## Rsc.Start field

Дата, когда назначенный ресурс запланирован начать работу над задачей.

```csharp
public static readonly Key<DateTime, RscKey> Start;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.Start.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Start, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Start: " + resource.Get(Rsc.Start));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


