---
title: "Calendar.WorkWeeks"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Calendar. Obtiene el objeto WorkWeekCollections. La colección de semanas laborables asociada al calendario"
type: docs
weight: 130
url: /es/net/aspose.tasks/calendar/workweeks/
---
## Calendar.WorkWeeks property

Obtiene el objeto WorkWeekCollections. La colección de semanas laborables asociada al calendario.

```csharp
public WorkWeekCollection WorkWeeks { get; }
```

## Ejemplos

Muestra cómo leer la información de la semana laboral.

```csharp
var project = new Project(DataDir + "WorkWithWorkWeekCollection.mpp");
var calendar = project.Calendars.GetByUid(1);

foreach (var workWeek in calendar.WorkWeeks)
{
    // Mostrar el nombre de la semana laboral, y las fechas de inicio y fin
    var name = workWeek.Name;
    var fromDate = workWeek.FromDate;
    var toDate = workWeek.ToDate;
    Console.WriteLine("Name: " + name);
    Console.WriteLine("From Date: " + fromDate);
    Console.WriteLine("To Date: " + toDate);

    // Estos datos tratan sobre el botón "Detalles." puedes establecer tiempos de trabajo especiales para un WeekDay especial o incluso marcarlo como no laborable.
    foreach (var day in workWeek.WeekDays)
    {
        // Puedes recorrer más a fondo los tiempos de trabajo y mostrarlos.
        foreach (var workingTime in day.WorkingTimes)
        {
            Console.WriteLine(workingTime.From);
            Console.WriteLine(workingTime.To);
        }
    }
}
```

### Ver también

* class [WorkWeekCollection](../../workweekcollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


