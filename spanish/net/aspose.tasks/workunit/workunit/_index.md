---
title: "WorkUnit.WorkUnit"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor WorkUnit. Inicializa una nueva instancia de la clase WorkUnit. Crea un nuevo objeto WorkUnit con las fechas From y To especificadas"
type: docs
weight: 10
url: /es/net/aspose.tasks/workunit/workunit/
---
## WorkUnit constructor

Inicializa una nueva instancia de la clase [`WorkUnit`](../). Crea un nuevo objeto WorkUnit con las fechas From y To especificadas.

```csharp
public WorkUnit(DateTime from, DateTime to)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| desde | DateTime | Fecha de inicio de las horas de trabajo. |
| a | DateTime | Fecha de finalización de las horas de trabajo. |

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


