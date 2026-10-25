---
title: "Calendar.Name"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Calendar. Obtiene o establece el nombre del calendario"
type: docs
weight: 90
url: /es/net/aspose.tasks/calendar/name/
---
## Calendar.Name property

Obtiene o establece el nombre del calendario.

```csharp
public string Name { get; set; }
```

## Ejemplos

Muestra cómo recuperar la información del calendario.

```csharp
var project = new Project(DataDir + "RetrieveCalendarInfo.mpp");

// Recuperar información de los calendarios
foreach (var calendar in project.Calendars)
{
    if (calendar.Name == null)
    {
        continue;
    }

    Console.WriteLine("Calendar UID: " + calendar.Uid);
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### Ver también

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


