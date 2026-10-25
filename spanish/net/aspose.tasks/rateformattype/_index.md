---
title: "Enumeración RateFormatType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enumeración Aspose.Tasks.RateFormatType. Especifica las unidades que usa Microsoft Project para mostrar una tarifa."
type: docs
weight: 1640
url: /es/net/aspose.tasks/rateformattype/
---
## RateFormatType enumeration

Especifica las unidades utilizadas por Microsoft Project para mostrar una tarifa.

```csharp
public enum RateFormatType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Undefined | `-1` | El valor no estaba definido en el archivo de proyecto original. |
| Minute | `0` | Minuto ("min") |
| Hour | `1` | Hora ("hr") |
| Day | `2` | Día ("day") |
| Week | `3` | Semana ("wk") |
| Month | `4` | Mes ("mo") |
| Year | `5` | Año ("yr") |
| MaterialResourceRate | `6` | Tarifa de recurso material (vacío) |

## Observaciones

Al exportar a XML, los valores Undefined se eliminarán del XML resultante.

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.StandardRateFormat.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.StandardRateFormat, RateFormatType.Hour);

Console.WriteLine("Standard Rate Format: " + resource.Get(Rsc.StandardRateFormat));
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


