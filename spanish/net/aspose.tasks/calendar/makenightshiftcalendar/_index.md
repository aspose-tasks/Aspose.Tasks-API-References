---
title: "Calendar.MakeNightShiftCalendar"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Calendar. Convierte un Calendar dado en Night Shift Calendar"
type: docs
weight: 20
url: /es/net/aspose.tasks/calendar/makenightshiftcalendar/
---
## Calendar.MakeNightShiftCalendar method

Convierte un Calendar dado en un Calendar de turno nocturno.

```csharp
public static Calendar MakeNightShiftCalendar(Calendar calendar)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| calendario | Calendar | Calendar para crear Night Shift Calendar. |

### Valor devuelto

Night Shift Calendar.

## Ejemplos

Muestra cómo crear un Night Shift Calendar.

```csharp
Project project = new Project();
var calendar = project.Calendars.Add("New calendar");
Calendar.MakeNightShiftCalendar(calendar);

var workingHours = calendar.GetWorkingTimes(new DateTime(2020, 4, 8));

// mostrar horas de trabajo
foreach (var wh in workingHours)
{
    Console.WriteLine("From: " + wh.From);
    Console.WriteLine("To: " + wh.To);
}
```

Muestra cómo transformar un calendario en un Night Shift Calendar.

```csharp
var project = new Project();

var calendar = project.Calendars.Add("Night Shift");
calendar = Calendar.MakeNightShiftCalendar(calendar);

var workingHours = calendar.GetWorkingTimes(new DateTime(2020, 4, 8));

// mostrar horas de trabajo
foreach (var wh in workingHours)
{
    Console.WriteLine("From: " + wh.From);
    Console.WriteLine("To: " + wh.To);
}
```

### Ver también

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


