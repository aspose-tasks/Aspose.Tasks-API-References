---
title: "Rsc.MaterialLabel"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Единица измерения материального ресурса"
type: docs
weight: 440
url: /ru/net/aspose.tasks/rsc/materiallabel/
---
## Rsc.MaterialLabel field

Единица измерения материалного ресурса.

```csharp
public static readonly Key<string, RscKey> MaterialLabel;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.MaterialLabel.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.MaterialLabel, "kg");

Console.WriteLine("Material Label: " + resource.Get(Rsc.MaterialLabel));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


