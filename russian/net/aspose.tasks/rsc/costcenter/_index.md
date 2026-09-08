---
title: "Rsc.CostCenter"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Указывает, к какому центру затрат должны быть отнесены расходы, начисленные на ресурс"
type: docs
weight: 230
url: /ru/net/aspose.tasks/rsc/costcenter/
---
## Rsc.CostCenter field

Указывает, к какому центру затрат должны быть отнесены расходы, начисленные ресурсом.

```csharp
public static readonly Key<string, RscKey> CostCenter;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.CostCenter.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostCenter, "Center");

Console.WriteLine("Cost Center: " + resource.Get(Rsc.CostCenter));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


