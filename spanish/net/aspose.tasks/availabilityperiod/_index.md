---
title: "Class AvailabilityPeriod"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.AvailabilityPeriod class. Representa un período cuando un recurso está disponible"
type: docs
weight: 80
url: /es/net/aspose.tasks/availabilityperiod/
---
## AvailabilityPeriod class

Representa un período en el que un recurso está disponible.

```csharp
public class AvailabilityPeriod
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [AvailabilityPeriod](availabilityperiod/#constructor)() | Inicializa una nueva instancia de `AvailabilityPeriod`. |
| [AvailabilityPeriod](availabilityperiod/#constructor_1)(DateTime, DateTime, double) | Inicializa una nueva instancia de `AvailabilityPeriod` con el rango de fechas especificado y unidades disponibles. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AvailableFrom](../../aspose.tasks/availabilityperiod/availablefrom/) { get; set; } | Obtiene o establece la fecha en que un recurso se vuelve disponible para el período especificado. |
| [AvailableTo](../../aspose.tasks/availabilityperiod/availableto/) { get; set; } | Obtiene o establece la última fecha en que un recurso está disponible para el período especificado. |
| [AvailableUnits](../../aspose.tasks/availabilityperiod/availableunits/) { get; set; } | Obtiene o establece el porcentaje de un recurso que está disponible durante el período especificado. |

## Ejemplos

Muestra cómo crear períodos de disponibilidad para un recurso.

```csharp
public void WorkWithAvailabilityPeriod()
{
    var project = new Project();
    var resource = project.Resources.Add("Work Resource");

    // Agregar períodos de disponibilidad al nuevo recurso
    IEnumerable<AvailabilityPeriod> periods = GetPeriods();
    foreach (var period in periods)
    {
        resource.AvailabilityPeriods.Add(period);
    }

    foreach (var period in resource.AvailabilityPeriods)
    {
        Console.WriteLine("Available From: " + period.AvailableFrom);
        Console.WriteLine("Available To: " + period.AvailableTo);
        Console.WriteLine("Available Units: " + period.AvailableUnits);
        Console.WriteLine();
    }
}

private static IEnumerable<AvailabilityPeriod> GetPeriods()
{
    var periods = new List<AvailabilityPeriod>(2);
    var period = new AvailabilityPeriod
    {
        AvailableFrom = new DateTime(2011, 12, 12),
        AvailableTo = new DateTime(2013, 12, 12),
        AvailableUnits = 0.99
    };

    periods.Add(period);

    var period2 = new AvailabilityPeriod
    {
        AvailableFrom = new DateTime(2013, 12, 12),
        AvailableTo = new DateTime(2015, 12, 12),
        AvailableUnits = 0.94
    };
    periods.Add(period2);
    return periods;
}
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


