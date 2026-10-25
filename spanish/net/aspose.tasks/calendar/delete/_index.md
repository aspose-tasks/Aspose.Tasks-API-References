---
title: "Calendar.Delete"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Calendar. Elimina el calendario del proyecto"
type: docs
weight: 140
url: /es/net/aspose.tasks/calendar/delete/
---
## Calendar.Delete method

Elimina el calendar del proyecto.

```csharp
public void Delete()
```

## Ejemplos

Muestra cómo eliminar un calendario de un proyecto.

```csharp
var project = new Project(DataDir + "BrokenCalendar.mpp");

// obtener el calendario por nombre
var calendar = project.Calendars.GetByName("Broken Calendar");

// eliminar el calendario
calendar.Delete();
```

### Ver también

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


