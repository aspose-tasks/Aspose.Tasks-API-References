---
title: "Rsc.IsCostResource"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Определяет, является ли ресурс ресурсом затрат"
type: docs
weight: 390
url: /ru/net/aspose.tasks/rsc/iscostresource/
---
## Rsc.IsCostResource field

Определяет, является ли ресурс ресурсом затрат.

```csharp
public static readonly Key<NullableBool, RscKey> IsCostResource;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.IsCostResource.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsCostResource, true);

Console.WriteLine("Is Cost Resource: " + resource.Get(Rsc.IsCostResource));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


