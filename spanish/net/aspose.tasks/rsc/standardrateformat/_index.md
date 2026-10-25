---
title: "Rsc.StandardRateFormat"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. Las unidades utilizadas por Microsoft Project para mostrar la tarifa estándar"
type: docs
weight: 630
url: /es/net/aspose.tasks/rsc/standardrateformat/
---
## Rsc.StandardRateFormat field

Las unidades utilizadas por Microsoft Project para mostrar la tarifa estándar.

```csharp
public static readonly Key<RateFormatType, RscKey> StandardRateFormat;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.StandardRateFormat.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.StandardRateFormat, RateFormatType.Hour);

Console.WriteLine("Standard Rate Format: " + resource.Get(Rsc.StandardRateFormat));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RateFormatType](../../rateformattype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


