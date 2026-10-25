---
title: "Clase WorkingTime"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.WorkingTime. Representa un tiempo de trabajo durante un día laborable."
type: docs
weight: 3660
url: /es/net/aspose.tasks/workingtime/
---
## WorkingTime class

Representa un tiempo de trabajo durante un día de la semana.

```csharp
public class WorkingTime
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [WorkingTime](workingtime/#constructor_1)(DateTime, DateTime) | Inicializa una nueva instancia de la clase `WorkingTime` con un intervalo con los tiempos de inicio y fin especificados. |
| [WorkingTime](workingtime/#constructor)(int, int) | Inicializa una nueva instancia de la clase `WorkingTime` con un elemento de intervalo con los tiempos de inicio y fin especificados. |
| [WorkingTime](workingtime/#constructor_2)(TimeSpan, TimeSpan) | Inicializa una nueva instancia de la clase `WorkingTime` con un elemento de intervalo con los tiempos de inicio y fin especificados. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [From](../../aspose.tasks/workingtime/from/) { get; } | Obtiene el comienzo de un tiempo de trabajo. |
| [To](../../aspose.tasks/workingtime/to/) { get; } | Obtiene el final de un tiempo de trabajo. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [Equals](../../aspose.tasks/workingtime/equals/)(object) | Comprueba que los objetos son iguales. |
| override [GetHashCode](../../aspose.tasks/workingtime/gethashcode/)() | Devuelve un valor de código hash para la instancia de la clase `WorkingTime`. |

## Ejemplos

Muestra cómo trabajar con información de tiempo de trabajo.

```csharp
public void WorkWithWorkingTime()
{
    var project = new Project();
    var calendar = CreateCalendar(project);
    project.Set(Prj.Calendar, calendar);

    Console.WriteLine("Work Week Number: " + calendar.WeekDays.Count);

    // Estos datos tratan sobre el botón "Detalles." puedes establecer tiempos de trabajo especiales para un WeekDay especial o incluso marcarlo como no laborable.
    List<WeekDay> weekDays = calendar.WeekDays.ToList();
    foreach (var day in weekDays)
    {
        Console.WriteLine(day.DayType.ToString());

        // Puedes recorrer más a fondo los tiempos de trabajo y mostrarlos.
        foreach (var workingTime in day.WorkingTimes)
        {
            Console.WriteLine(workingTime.From);
            Console.WriteLine(workingTime.To);
        }
    }
}

public static Calendar CreateCalendar(Project project)
{
    var calendar = project.Calendars.Add("MyCalendar", project.Calendars.GetByName("Standard"));
    var workingTimes = new List<WorkingTime>
                           {
                               new WorkingTime(new DateTime(1, 1, 1, 9, 0, 0), new DateTime(1, 1, 1, 12, 0, 0)),
                               new WorkingTime(new DateTime(1, 1, 1, 13, 0, 0), new DateTime(1, 1, 1, 18, 0, 0))
                           };

    calendar.WeekDays.Add(new WeekDay(DayType.Monday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Tuesday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Wednesday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Thursday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Friday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
    calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

    return calendar;
}
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


