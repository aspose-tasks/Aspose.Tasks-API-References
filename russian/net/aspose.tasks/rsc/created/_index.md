---
title: "Rsc.Created"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Дата и время, когда ресурс был добавлен в проект"
type: docs
weight: 260
url: /ru/net/aspose.tasks/rsc/created/
---
## Rsc.Created field

Дата и время, когда ресурс был добавлен в проект.

```csharp
public static readonly Key<DateTime, RscKey> Created;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.Created.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Created, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Created: " + resource.Get(Rsc.Created));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


