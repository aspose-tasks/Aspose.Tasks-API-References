---
title: "Clase WorkUnit"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.WorkUnit. Representa horas de trabajo"
type: docs
weight: 3630
url: /es/net/aspose.tasks/workunit/
---
## WorkUnit class

Representa horas de trabajo.

```csharp
public class WorkUnit
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [WorkUnit](workunit/)(DateTime, DateTime) | Inicializa una nueva instancia de la clase `WorkUnit`. Crea un nuevo objeto WorkUnit con las fechas From y To especificadas. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [From](../../aspose.tasks/workunit/from/) { get; set; } | Obtiene o establece la fecha From. |
| [To](../../aspose.tasks/workunit/to/) { get; set; } | Obtiene o establece la fecha To. |
| [WorkingHours](../../aspose.tasks/workunit/workinghours/) { get; set; } | Obtiene o establece la duración de las horas de trabajo. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


