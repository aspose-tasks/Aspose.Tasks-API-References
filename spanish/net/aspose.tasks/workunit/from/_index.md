---
title: "WorkUnit.From"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad WorkUnit. Obtiene o establece la fecha From"
type: docs
weight: 20
url: /es/net/aspose.tasks/workunit/from/
---
## WorkUnit.From property

Obtiene o establece la fecha From.

```csharp
public DateTime From { get; set; }
```

## Ejemplos

Muestra cómo trabajar con la información de la unidad de trabajo.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// obtén horas de trabajo para una fecha específica
var workUnit = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0), new DateTime(2020, 4, 9, 17, 0, 0));

Console.WriteLine("From: " + workUnit.From);
Console.WriteLine("To: " + workUnit.To);
Console.WriteLine("Working hours: " + workUnit.WorkingHours);
```

### Ver también

* class [WorkUnit](../)
* namespace [Aspose.Tasks](../../workunit/)
* assembly [Aspose.Tasks](../../../)


