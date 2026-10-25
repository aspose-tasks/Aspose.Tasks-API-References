---
title: "Rsc.Finish"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Дата, когда ресурс запланирован завершить работу над всеми назначенными задачами"
type: docs
weight: 290
url: /ru/net/aspose.tasks/rsc/finish/
---
## Rsc.Finish field

Дата, когда ресурс планирует завершить работу над всеми назначенными задачами.

```csharp
public static readonly Key<DateTime, RscKey> Finish;
```

## Примеры

Показывает, как прочитать/записать свойство Rsc.Finish.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Finish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Finish: " + resource.Get(Rsc.Finish));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


