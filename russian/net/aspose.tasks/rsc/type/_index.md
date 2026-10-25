---
title: "Rsc.Type"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Тип ресурса"
type: docs
weight: 660
url: /ru/net/aspose.tasks/rsc/type/
---
## Rsc.Type field

Тип ресурса.

```csharp
public static readonly Key<ResourceType, RscKey> Type;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.Type.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Type, ResourceType.Work);

Console.WriteLine("Type: " + resource.Get(Rsc.Type));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [ResourceType](../../resourcetype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


