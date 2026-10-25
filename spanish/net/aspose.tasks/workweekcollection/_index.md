---
title: "Clase WorkWeekCollection"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.WorkWeekCollection. Representa una colección de objetos WorkWeek."
type: docs
weight: 3650
url: /es/net/aspose.tasks/workweekcollection/
---
## WorkWeekCollection class

Representa una colección de objetos [`WorkWeek`](../workweek/).

```csharp
public class WorkWeekCollection : IList<WorkWeek>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.tasks/workweekcollection/count/) { get; } | Obtiene el número de objetos contenidos en este objeto `WorkWeekCollection`. |
| [Item](../../aspose.tasks/workweekcollection/item/) { get; set; } | Devuelve el elemento en el índice especificado. |
| [ParentCalendar](../../aspose.tasks/workweekcollection/parentcalendar/) { get; } | Obtiene el calendario principal. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.tasks/workweekcollection/add/)(WorkWeek) | Agrega una instancia de WorkWeek a este objeto de colección. |
| [GetEnumerator](../../aspose.tasks/workweekcollection/getenumerator/)() | Devuelve un enumerador para esta colección. |
| [ToList](../../aspose.tasks/workweekcollection/tolist/)() | Convierte el objeto WorkWeekCollection en una lista de objetos [`WorkWeek`](../workweek/). |

## Ejemplos

Muestra cómo crear una semana laboral personalizada para un calendario.

```csharp
var project = new Project();
var calendar = project.Calendars.Add("Standard");
Calendar.MakeStandardCalendar(calendar);

var item = new WorkWeek();
item.Name = "My Work Week";
item.FromDate = new DateTime(2020, 4, 13, 8, 0, 0);
item.ToDate = new DateTime(2020, 4, 17, 17, 0, 0);
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));
item.WeekDays.Add(new WeekDay(DayType.Saturday));
item.WeekDays.Add(new WeekDay(DayType.Sunday));
calendar.WorkWeeks.Add(item);

Console.WriteLine("Work Weeks Count: " + calendar.WorkWeeks.Count);
foreach (var workWeek in calendar.WorkWeeks)
{
    // Muestra el nombre de la semana de trabajo, el nombre del calendario padre, y las fechas de inicio y fin.
    Console.WriteLine("Name: " + workWeek.Name);
    Console.WriteLine("Parent calendar name: " + calendar.Name);
    Console.WriteLine("From Date: " + workWeek.FromDate);
    Console.WriteLine("To Date: " + workWeek.ToDate);
    Console.WriteLine();

    // Estos datos tratan sobre el botón "Detalles." puedes establecer tiempos de trabajo especiales para un WeekDay especial o incluso marcarlo como no laborable.
    List<WeekDay> weekDays = workWeek.WeekDays.ToList();
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

    Console.WriteLine();
}
```

### Ver también

* class [WorkWeek](../workweek/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


