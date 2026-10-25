---
title: "Rsc.Name"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Имя ресурса"
type: docs
weight: 460
url: /ru/net/aspose.tasks/rsc/name/
---
## Rsc.Name field

Имя ресурса.

```csharp
public static readonly Key<string, RscKey> Name;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.Name.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Name, "John Smith");

Console.WriteLine("Name: " + resource.Get(Rsc.Name));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


