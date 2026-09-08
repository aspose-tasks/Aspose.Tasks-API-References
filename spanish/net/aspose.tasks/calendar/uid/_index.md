---
title: "Calendar.Uid"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Calendar. Obtiene o establece el identificador único del calendario"
type: docs
weight: 110
url: /es/net/aspose.tasks/calendar/uid/
---
## Calendar.Uid property

Obtiene o establece el identificador único del calendario.

```csharp
public int Uid { get; set; }
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


