---
title: "Calendar.Make24HourCalendar"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Calendar. Convierte un Calendar dado en un 24Hour Calendar. 24Hours Calendar es un Calendar en el que cada día de la semana trabaja con Roundtheclock horas laborables."
type: docs
weight: 10
url: /es/net/aspose.tasks/calendar/make24hourcalendar/
---
## Calendar.Make24HourCalendar method

Convierte un Calendar dado en un Calendar de 24 horas. El Calendar de 24 horas es un calendario en el que cada día de la semana trabaja con horarios continuos.

```csharp
public static Calendar Make24HourCalendar(Calendar calendar)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| calendario | Calendar | Calendario para crear un Calendario de 24 Horas a partir de. |

### Valor devuelto

Calendario de 24 Horas.

## Ejemplos

Muestra cómo crear un calendario de 24 horas.

```csharp
Project project = new Project();
var calendar = project.Calendars.Add("New calendar");
Calendar.Make24HourCalendar(calendar);

var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0));

// Se imprimirán 24 horas
Console.WriteLine("Hours: " + workingHours.TotalHours);
```

Muestra cómo transformar un calendario nuevo en un calendario de 24 horas.

```csharp
var project = new Project();

var calendar = project.Calendars.Add("24 Hours");
calendar = Calendar.Make24HourCalendar(calendar);

var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0));

// Se imprimirán 24 horas
Console.WriteLine("Hours: " + workingHours.TotalHours);
```

### Ver también

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


