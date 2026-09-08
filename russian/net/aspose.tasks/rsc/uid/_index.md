---
title: "Rsc.Uid"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Уникальный идентификатор ресурса."
type: docs
weight: 670
url: /ru/net/aspose.tasks/rsc/uid/
---
## Rsc.Uid field

Уникальный идентификатор ресурса.

```csharp
public static readonly Key<int, RscKey> Uid;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.Uid.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Uid, 99);

Console.WriteLine("Uid: " + resource.Get(Rsc.Uid));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


