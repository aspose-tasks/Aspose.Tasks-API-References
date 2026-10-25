---
title: "Calendar.IsBaselineCalendar"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Calendar. Obtiene o establece un valor que indica si el calendario es un calendario de línea base"
type: docs
weight: 80
url: /es/net/aspose.tasks/calendar/isbaselinecalendar/
---
## Calendar.IsBaselineCalendar property

Obtiene o establece un valor que indica si el calendario es un calendario de línea base.

```csharp
public bool IsBaselineCalendar { get; set; }
```

## Ejemplos

Muestra cómo comprobar si un calendario es un calendario de línea base o no.

```csharp
var project = new Project(DataDir + "IsBaselineCalendar.mpp");

var calendar = project.Calendars.GetByUid(3);

Console.WriteLine("Is baseline calendar: " + calendar.IsBaselineCalendar);
```

### Ver también

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


