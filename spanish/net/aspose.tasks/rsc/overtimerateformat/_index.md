---
title: "Rsc.OvertimeRateFormat"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. Las unidades que usa Microsoft Project para mostrar la tarifa de horas extra"
type: docs
weight: 520
url: /es/net/aspose.tasks/rsc/overtimerateformat/
---
## Rsc.OvertimeRateFormat field

Las unidades utilizadas por Microsoft Project para mostrar la tarifa de horas extra.

```csharp
public static readonly Key<RateFormatType, RscKey> OvertimeRateFormat;
```

## Ejemplos

Muestra cómo leer los valores de horas extra del recurso.

```csharp
var project = new Project(DataDir + "ResourceOvertime.mpp");

// Mostrar parámetros relacionados con horas extra para todos los recursos
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) == null)
    {
        continue;
    }

    Console.WriteLine(res.Get(Rsc.OvertimeCost));
    Console.WriteLine(res.Get(Rsc.OvertimeWork).ToString());
    Console.WriteLine(res.Get(Rsc.OvertimeRateFormat).ToString());
}
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RateFormatType](../../rateformattype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


