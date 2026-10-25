---
title: "WorkWeek.WeekDays"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad WorkWeek. Obtiene los días de la semana"
type: docs
weight: 50
url: /es/net/aspose.tasks/workweek/weekdays/
---
## WorkWeek.WeekDays property

Obtiene los días de la semana.

```csharp
public WeekDayCollection WeekDays { get; }
```

## Ejemplos

Muestra cómo leer la información de la semana de trabajo del proyecto.

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

Console.WriteLine("Work Week Number: " + calendar.WeekDays.Count);
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

* class [WeekDayCollection](../../weekdaycollection/)
* class [WorkWeek](../)
* namespace [Aspose.Tasks](../../workweek/)
* assembly [Aspose.Tasks](../../../)


