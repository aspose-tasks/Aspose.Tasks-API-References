---
title: "Rsc.CostVariance"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Разница между базовой стоимостью и общей стоимостью ресурса"
type: docs
weight: 250
url: /ru/net/aspose.tasks/rsc/costvariance/
---
## Rsc.CostVariance field

Разница между базовой стоимостью и общей стоимостью ресурса.

```csharp
public static readonly Key<double, RscKey> CostVariance;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.CostVariance.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostVariance, 10);

Console.WriteLine("Cost Variance: " + resource.Get(Rsc.CostVariance));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


