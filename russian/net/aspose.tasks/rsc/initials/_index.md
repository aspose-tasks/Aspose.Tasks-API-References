---
title: "Rsc.Initials"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Инициалы ресурса"
type: docs
weight: 370
url: /ru/net/aspose.tasks/rsc/initials/
---
## Rsc.Initials field

Инициалы ресурса.

```csharp
public static readonly Key<string, RscKey> Initials;
```

## Примеры

Показывает, как прочитать/записать свойство Rsc.Initials.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Initials, "R");

Console.WriteLine("Initials: " + resource.Get(Rsc.Initials));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


