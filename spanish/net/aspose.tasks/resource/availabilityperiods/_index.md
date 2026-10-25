---
title: "Resource.AvailabilityPeriods"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Resource. Obtiene una instancia de la clase AvailabilityPeriodCollection. La colección de períodos durante los cuales un recurso está disponible"
type: docs
weight: 130
url: /es/net/aspose.tasks/resource/availabilityperiods/
---
## Resource.AvailabilityPeriods property

Obtiene una instancia de la clase [`AvailabilityPeriodCollection`](../../availabilityperiodcollection/). La colección de períodos durante los cuales un recurso está disponible.

```csharp
public AvailabilityPeriodCollection AvailabilityPeriods { get; }
```

## Ejemplos

Muestra cómo agregar un período de disponibilidad para un recurso.

```csharp
var project = new Project();
var resource = project.Resources.Add("Resource");

var availabilityPeriod = new AvailabilityPeriod
{
    AvailableFrom = new DateTime(2020, 4, 1, 8, 0, 0),
    AvailableTo = new DateTime(2020, 4, 1, 17, 0, 0),
    AvailableUnits = 2d
};
resource.AvailabilityPeriods.Add(availabilityPeriod);

var availabilityPeriod2 = new AvailabilityPeriod
{
    AvailableFrom = new DateTime(2020, 4, 2, 8, 0, 0),
    AvailableTo = new DateTime(2020, 4, 2, 17, 0, 0),
    AvailableUnits = 3d
};
resource.AvailabilityPeriods.Add(availabilityPeriod2);
```

### Ver también

* class [AvailabilityPeriodCollection](../../availabilityperiodcollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


