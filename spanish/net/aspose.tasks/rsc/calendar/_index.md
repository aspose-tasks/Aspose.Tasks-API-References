---
title: "Rsc.Calendar"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. El calendario de un recurso"
type: docs
weight: 190
url: /es/net/aspose.tasks/rsc/calendar/
---
## Rsc.Calendar field

El calendario de un recurso.

```csharp
public static readonly Key<Calendar, RscKey> Calendar;
```

## Ejemplos

Muestra cómo obtener/establecer un calendario de recurso.

```csharp
var project = new Project(DataDir + "ResourceCalendar.mpp");
var res = project.Resources.Add("Resource1");

// Agregar calendario estándar y asignarlo al recurso
var cal = project.Calendars.Add("Resource1");
res.Set(Rsc.Calendar, cal);

// Mostrar el nombre del calendario base para todos los recursos
foreach (var resource in project.Resources)
{
    if (resource.Get(Rsc.Name) != null)
    {
        Console.WriteLine(resource.Get(Rsc.Calendar).BaseCalendar.Name);
    }
}
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


