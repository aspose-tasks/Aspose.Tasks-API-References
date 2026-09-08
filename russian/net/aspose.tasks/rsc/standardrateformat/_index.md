---
title: "Rsc.StandardRateFormat"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Единицы измерения, используемые Microsoft Project для отображения стандартной ставки"
type: docs
weight: 630
url: /ru/net/aspose.tasks/rsc/standardrateformat/
---
## Rsc.StandardRateFormat field

Единицы, используемые Microsoft Project для отображения стандартной ставки.

```csharp
public static readonly Key<RateFormatType, RscKey> StandardRateFormat;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.StandardRateFormat.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.StandardRateFormat, RateFormatType.Hour);

Console.WriteLine("Standard Rate Format: " + resource.Get(Rsc.StandardRateFormat));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RateFormatType](../../rateformattype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


