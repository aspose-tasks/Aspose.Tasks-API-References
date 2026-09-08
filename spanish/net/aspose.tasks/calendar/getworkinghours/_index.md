---
title: "Calendar.GetWorkingHours"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Calendar. Devuelve WorkUnit, Inicio, Fin y Duración de las horas laborables para el intervalo de fecha y hora especificado"
type: docs
weight: 220
url: /es/net/aspose.tasks/calendar/getworkinghours/
---
## GetWorkingHours(DateTime, DateTime) {#getworkinghours}

Devuelve WorkUnit - Inicio, Fin y Duración de las horas de trabajo para el intervalo de fecha y hora especificado.

```csharp
public WorkUnit GetWorkingHours(DateTime start, DateTime finish)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inicio | DateTime | Fecha de inicio del intervalo. |
| finalizar | DateTime | Fecha de finalización del intervalo. |

### Valor devuelto

Instancia de la clase [`WorkUnit`](../../workunit/) que contiene Inicio, Fin y Duración de las horas de trabajo.

## Ejemplos

Muestra cómo obtener las horas laborables para fechas específicas.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// obtén horas de trabajo para una fecha específica
var workUnit = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0), new DateTime(2020, 4, 9, 17, 0, 0));

// Se imprimirán 16 horas
Console.WriteLine(workUnit.WorkingHours);
```

### Ver también

* class [WorkUnit](../../workunit/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetWorkingHours(DateTime) {#getworkinghours_1}

Devuelve la cantidad de horas laborables en la fecha especificada.

```csharp
public TimeSpan GetWorkingHours(DateTime dt)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dt | DateTime | La fecha para la que se obtienen las horas de trabajo. |

### Valor devuelto

Horas de trabajo en la fecha especificada.

## Ejemplos

Muestra cómo obtener las horas laborables para una fecha específica.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// obtén horas de trabajo para una fecha específica
var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 10));

// Se imprimirán 8 horas
Console.WriteLine(workingHours.Hours);
```

### Ver también

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


