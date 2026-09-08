---
title: "Rsc.Guid"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Содержит сгенерированный уникальный идентификационный код ресурса"
type: docs
weight: 310
url: /ru/net/aspose.tasks/rsc/guid/
---
## Rsc.Guid field

Содержит сгенерированный уникальный идентификационный код ресурса.

```csharp
public static readonly Key<string, RscKey> Guid;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.Guid.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Guid, "1385689c-2dd1-4114-935b-054beb6fbbbe");

Console.WriteLine("Guid: " + resource.Get(Rsc.Guid));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


