---
title: "Rsc.Id"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Идентификатор позиции ресурса в списке ресурсов"
type: docs
weight: 350
url: /ru/net/aspose.tasks/rsc/id/
---
## Rsc.Id field

Идентификатор позиции ресурса в списке ресурсов.

```csharp
public static readonly Key<int, RscKey> Id;
```

## Примеры

Показывает, как прочитать/записать свойство Rsc.Id.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Id, 987);

Console.WriteLine("Id: " + resource.Get(Rsc.Id));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


