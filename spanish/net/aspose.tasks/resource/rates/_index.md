---
title: "Resource.Rates"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Resource. Obtiene una instancia de la clase RateCollection para este objeto. La colección de períodos y tarifas asociados a cada uno"
type: docs
weight: 640
url: /es/net/aspose.tasks/resource/rates/
---
## Resource.Rates property

Obtiene una instancia de la clase [`RateCollection`](../../ratecollection/) para este objeto. La colección de períodos y tarifas asociados a cada uno.

```csharp
public RateCollection Rates { get; }
```

## Ejemplos

Muestra cómo leer las tarifas del recurso.

```csharp
var project = new Project();
var resource = project.Resources.Add();
resource.Set(Rsc.Uid, 1);
resource.Set(Rsc.Name, "Test Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);
resource.Set(Rsc.Work, project.GetDuration(2d, TimeUnitType.Hour));
resource.Set(Rsc.StandardRate, 20m);

var rate1 = resource.Rates.Add(new DateTime(2019, 1, 1, 8, 0, 0));
rate1.RatesTo = new DateTime(2019, 11, 11, 17, 0, 0);
rate1.StandardRate = 5m;
rate1.StandardRateFormat = RateFormatType.Hour;

var rate2 = resource.Rates.Add(new DateTime(2019, 11, 12, 8, 0, 0));
rate2.RatesTo = new DateTime(2019, 12, 31, 17, 0, 0);
rate2.StandardRate = 10m;
rate2.StandardRateFormat = RateFormatType.Hour;

// iterar sobre tarifas
foreach (KeyValuePair<RateType, RateByDateCollection> rate in resource.Rates)
{
    foreach (KeyValuePair<DateTime, Rate> pair in rate.Value)
    {
        Console.WriteLine(pair.Value.RatesFrom);
        Console.WriteLine(pair.Value.RatesTo);
    }
}
```

### Ver también

* class [RateCollection](../../ratecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


