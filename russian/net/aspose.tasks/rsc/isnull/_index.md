---
title: "Rsc.IsNull"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Определяет, является ли ресурс null"
type: docs
weight: 420
url: /ru/net/aspose.tasks/rsc/isnull/
---
## Rsc.IsNull field

Определяет, является ли ресурс пустым (null).

```csharp
public static readonly Key<NullableBool, RscKey> IsNull;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.IsNull.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsNull, true);

Console.WriteLine("Is Null: " + resource.Get(Rsc.IsNull));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


