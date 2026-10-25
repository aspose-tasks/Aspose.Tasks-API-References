---
title: "Rsc.Code"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Код или другая информация о ресурсе"
type: docs
weight: 210
url: /ru/net/aspose.tasks/rsc/code/
---
## Rsc.Code field

Код или другая информация о ресурсе.

```csharp
public static readonly Key<string, RscKey> Code;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.Code.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Code, "555292");

Console.WriteLine("Code: " + resource.Get(Rsc.Code));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


