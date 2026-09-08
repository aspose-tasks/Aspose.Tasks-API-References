---
title: "Rsc.MaxUnits"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Максимальное количество единиц, представляющих максимальную ёмкость, для которой ресурс доступен для выполнения любых задач в текущий период времени"
type: docs
weight: 450
url: /ru/net/aspose.tasks/rsc/maxunits/
---
## Rsc.MaxUnits field

Максимальное количество единиц, представляющих максимальную емкость, в которой ресурс доступен для выполнения любых задач в текущий период времени.

```csharp
public static readonly Key<double, RscKey> MaxUnits;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.MaxUnits.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.MaxUnits, 2);

Console.WriteLine("Max Units: " + resource.Get(Rsc.MaxUnits));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


