---
title: "Calendar.PrimaveraProperties"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Calendar. Obtiene un objeto que contiene propiedades específicas de Primavera para un calendario leído de formatos Primavera."
type: docs
weight: 100
url: /es/net/aspose.tasks/calendar/primaveraproperties/
---
## Calendar.PrimaveraProperties property

Obtiene un objeto que contiene propiedades específicas de Primavera para un calendario leído de formatos Primavera.

```csharp
public PrimaveraCalendarProperties PrimaveraProperties { get; }
```

## Ejemplos

Muestra cómo leer un proyecto de un archivo Primavera y examinar las propiedades específicas de Primavera del calendario.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 4861;

// Devuelve el proyecto con UID especial.
var project = new Project(DataDir + "ScheduleOptions.xer", options);

var calendar = project.Calendars.GetByUid(178);

Console.WriteLine("Hours per day in '{0}' : {1}", calendar.Name, calendar.PrimaveraProperties.HoursPerDay);
```

### Ver también

* class [PrimaveraCalendarProperties](../../primaveracalendarproperties/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


