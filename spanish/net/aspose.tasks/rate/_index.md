---
title: "Clase Rate"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Rate. Representa una definición de un período de tiempo y tarifas aplicables a un recurso durante ese período"
type: docs
weight: 1610
url: /es/net/aspose.tasks/rate/
---
## Rate class

Representa una definición de un período de tiempo y tarifas aplicables a un recurso durante ese período.

```csharp
public class Rate
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CostPerUse](../../aspose.tasks/rate/costperuse/) { get; set; } | Obtiene o establece el costo por uso de un recurso. Este valor se recupera de la fecha actual si existe una tabla de tarifas para un recurso. |
| [OvertimeRate](../../aspose.tasks/rate/overtimerate/) { get; set; } | Obtiene o establece la tarifa de horas extra por hora para un recurso. |
| [OvertimeRateFormat](../../aspose.tasks/rate/overtimerateformat/) { get; set; } | Obtiene o establece las unidades utilizadas por Microsoft Project para mostrar la tarifa de horas extra. |
| [RatesFrom](../../aspose.tasks/rate/ratesfrom/) { get; set; } | Obtiene o establece la fecha en que una tarifa entra en vigor. |
| [RatesTo](../../aspose.tasks/rate/ratesto/) { get; set; } | Obtiene o establece la última fecha en que una tarifa es efectiva. |
| [RateTable](../../aspose.tasks/rate/ratetable/) { get; set; } | Obtiene o establece el identificador único de una tabla de tarifas para un recurso. |
| [StandardRate](../../aspose.tasks/rate/standardrate/) { get; set; } | Obtiene o establece la tarifa estándar por hora para un recurso. |
| [StandardRateFormat](../../aspose.tasks/rate/standardrateformat/) { get; set; } | Obtiene o establece las unidades utilizadas por Microsoft Project para mostrar la tarifa estándar. |

## Ejemplos

Muestra cómo trabajar con tarifas de recursos.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);
resource.Set(Rsc.Work, project.GetDuration(2d, TimeUnitType.Hour));
resource.Set(Rsc.StandardRate, 20m);

var rate1 = resource.Rates.Add(new DateTime(2019, 1, 1, 8, 0, 0));
rate1.RateTable = RateType.A;
rate1.RatesFrom = new DateTime(2019, 1, 1, 8, 0, 0);
rate1.RatesTo = new DateTime(2019, 11, 11, 17, 0, 0);
rate1.StandardRate = 5m;
rate1.StandardRateFormat = RateFormatType.Hour;
rate1.OvertimeRate = 10m;
rate1.OvertimeRateFormat = RateFormatType.Hour;

var rate2 = resource.Rates.Add(new DateTime(2019, 11, 12, 8, 0, 0));
rate2.RatesTo = new DateTime(2019, 12, 31, 17, 0, 0);
rate2.StandardRate = 10m;
rate2.StandardRateFormat = RateFormatType.Hour;
rate2.CostPerUse = 2m;

// trabajar con el proyecto...
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


