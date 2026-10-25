---
title: "Rsc.AccrueAt"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Rsc field. Определяет, как и когда стандартные и сверхурочные затраты ресурса должны быть начислены или отложены к стоимости задачи"
type: docs
weight: 10
url: /ru/net/aspose.tasks/rsc/accrueat/
---
## Rsc.AccrueAt field

Определяет, как и когда стандартные и сверхурочные затраты ресурсов начисляются или учитываются в стоимости задачи.

```csharp
public static readonly Key<CostAccrualType, RscKey> AccrueAt;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.AccrueAt.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AccrueAt, CostAccrualType.End);

Console.WriteLine("Accrue At: " + resource.Get(Rsc.AccrueAt));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [CostAccrualType](../../costaccrualtype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


