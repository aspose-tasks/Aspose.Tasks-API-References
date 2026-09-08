---
title: "Rsc.Inactive"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Определяет, был ли ресурс сделан неактивным пользователем с административными правами"
type: docs
weight: 360
url: /ru/net/aspose.tasks/rsc/inactive/
---
## Rsc.Inactive field

Определяет, был ли ресурс сделан неактивным пользователем с административными правами.

```csharp
public static readonly Key<NullableBool, RscKey> Inactive;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.Inactive.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Inactive, true);

Console.WriteLine("Inactive: " + resource.Get(Rsc.Inactive));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


