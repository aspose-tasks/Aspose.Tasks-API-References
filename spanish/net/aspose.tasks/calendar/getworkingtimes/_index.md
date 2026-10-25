---
title: "Calendar.GetWorkingTimes"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Calendar. Devuelve WorkingTimeCollection de horarios de trabajo para la fecha especificada"
type: docs
weight: 240
url: /es/net/aspose.tasks/calendar/getworkingtimes/
---
## Calendar.GetWorkingTimes method

Devuelve [`WorkingTimeCollection`](../../workingtimecollection/) de tiempos laborables para la fecha especificada.

```csharp
public WorkingTimeCollection GetWorkingTimes(DateTime dt)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dt | DateTime | La fecha para la que se obtienen los tiempos de trabajo. |

### Valor devuelto

Colección de instancias de [`WorkingTime`](../../workingtime/).

## Ejemplos

Muestra cómo obtener horarios de trabajo para una fecha específica.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// obtener horarios de trabajo para una fecha específica
var workingTimes = calendar.GetWorkingTimes(new DateTime(2020, 4, 8, 8, 0, 0));

// Se imprimirán 16 horas
foreach (var workingTime in workingTimes)
{
    Console.WriteLine("From: " + workingTime.From);
    Console.WriteLine("To: " + workingTime.To);
}
```

### Ver también

* class [WorkingTimeCollection](../../workingtimecollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


