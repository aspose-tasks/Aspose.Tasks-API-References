---
title: "Rsc.IsGeneric"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Определяет, является ли ресурс универсальным или нет"
type: docs
weight: 410
url: /ru/net/aspose.tasks/rsc/isgeneric/
---
## Rsc.IsGeneric field

Определяет, является ли ресурс общим или нет.

```csharp
public static readonly Key<NullableBool, RscKey> IsGeneric;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.IsGeneric.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsGeneric, true);

Console.WriteLine("Is Generic: " + resource.Get(Rsc.IsGeneric));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


