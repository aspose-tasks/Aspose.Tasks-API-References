---
title: "Calendar.IsDayWorking"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Calendar. Determina si el día especificado es laborable según el calendario"
type: docs
weight: 260
url: /es/net/aspose.tasks/calendar/isdayworking/
---
## Calendar.IsDayWorking method

Determina si el día especificado es un día laborable según el calendario.

```csharp
public bool IsDayWorking(DateTime dt)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dt | DateTime | La fecha para comprobar si el día es laborable. |

### Valor devuelto

Verdadero si el día es laborable.

## Ejemplos

Muestra cómo calcular las horas laborables.

```csharp
var project = new Project(DataDir + "CalculateWorkHours.mpp");

// Acceder a la tarea por ID
var task = project.RootTask.Children.GetById(1);

// Acceder al calendario y sus fechas de inicio y fin
var taskCalendar = task.Get(Tsk.Calendar);
var startDate = task.Get(Tsk.Start);
var endDate = task.Get(Tsk.Finish);

// Acceder al recurso y su calendario
var resource = project.Resources.GetByUid(1);
var resourceCalendar = resource.Get(Rsc.Calendar);

TimeSpan timeSpan;

// Obtener duración en minutos
double durationInMins = 0;
var tempDate = startDate;
while (tempDate < endDate)
{
    if (taskCalendar.IsDayWorking(tempDate) && resourceCalendar.IsDayWorking(tempDate))
    {
        timeSpan = taskCalendar.GetWorkingHours(tempDate);
        durationInMins += timeSpan.TotalMinutes;
    }

    tempDate = tempDate.AddDays(1);
}

tempDate = startDate;

// Obtener duración en horas
double durationInHours = 0;
while (tempDate < endDate)
{
    if (taskCalendar.IsDayWorking(tempDate) && resourceCalendar.IsDayWorking(tempDate))
    {
        timeSpan = taskCalendar.GetWorkingHours(tempDate);
        durationInHours += timeSpan.TotalHours;
    }

    tempDate = tempDate.AddDays(1);
}

// Obtener duración en días
double durationInDays = 0;
tempDate = startDate;
while (tempDate < endDate)
{
    if (taskCalendar.IsDayWorking(tempDate) && resourceCalendar.IsDayWorking(tempDate))
    {
        timeSpan = taskCalendar.GetWorkingHours(tempDate);
        if (timeSpan.TotalHours > 0)
        {
            durationInDays += timeSpan.TotalDays * (24 / timeSpan.TotalHours);
        }
    }

    tempDate = tempDate.AddDays(1);
}

Console.WriteLine("Duration in Minutes = " + durationInMins);
Console.WriteLine("Duration in Hours = " + durationInHours);
Console.WriteLine("Duration in Days = " + durationInDays);
```

### Ver también

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


