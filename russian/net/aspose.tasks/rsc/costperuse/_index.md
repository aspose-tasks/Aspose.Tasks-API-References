---
title: "Rsc.CostPerUse"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Стоимость, начисляемая каждый раз при использовании ресурса"
type: docs
weight: 240
url: /ru/net/aspose.tasks/rsc/costperuse/
---
## Rsc.CostPerUse field

Стоимость, начисляемая каждый раз при использовании ресурса.

```csharp
public static readonly Key<decimal, RscKey> CostPerUse;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.CostPerUse.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostPerUse, 9);

Console.WriteLine("Cost Per Use: " + resource.Get(Rsc.CostPerUse));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


