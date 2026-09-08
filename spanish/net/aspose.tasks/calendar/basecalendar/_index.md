---
title: "Calendar.BaseCalendar"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Calendar. Obtiene o establece el calendario base del que depende este calendario. Sólo aplicable si el calendario no es un calendario base"
type: docs
weight: 40
url: /es/net/aspose.tasks/calendar/basecalendar/
---
## Calendar.BaseCalendar property

Obtiene o establece el calendario base del cual depende este calendario. Solo aplicable si el calendario no es un calendario base.

```csharp
public Calendar BaseCalendar { get; set; }
```

## Ejemplos

Muestra cómo trabajar con un calendario base del calendario del recurso.

```csharp
var project = new Project(DataDir + "ResourceCalendar.mpp");
var resource = project.Resources.Add("Resource1");

// Agregar calendario estándar y asignarlo al recurso
var calendar = project.Calendars.Add("Resource1");
resource.Set(Rsc.Calendar, calendar);

// Mostrar el nombre del calendario base para todos los recursos
foreach (var rsc in project.Resources)
{
    if (rsc.Get(Rsc.Name) != null)
    {
        Console.WriteLine(rsc.Get(Rsc.Calendar).BaseCalendar.Name);
    }
}
```

### Ver también

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


