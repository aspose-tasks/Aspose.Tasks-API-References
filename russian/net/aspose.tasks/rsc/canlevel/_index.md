---
title: "Rsc.CanLevel"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Rsc field. Определяет, можно ли выполнить выравнивание ресурсов для ресурса"
type: docs
weight: 200
url: /ru/net/aspose.tasks/rsc/canlevel/
---
## Rsc.CanLevel field

Определяет, можно ли выполнить выравнивание ресурсов для данного ресурса.

```csharp
public static readonly Key<NullableBool, RscKey> CanLevel;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.CanLevel.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CanLevel, true);

Console.WriteLine("Can Level: " + resource.Get(Rsc.CanLevel));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


