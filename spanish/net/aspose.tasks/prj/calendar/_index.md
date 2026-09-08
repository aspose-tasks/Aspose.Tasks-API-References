---
title: "Prj.Calendar"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. El calendario del proyecto"
type: docs
weight: 90
url: /es/net/aspose.tasks/prj/calendar/
---
## Prj.Calendar field

El calendario del proyecto.

```csharp
public static readonly Key<Calendar, PrjKey> Calendar;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Prj.Calendar.

```csharp
var project = new Project();
var calendar = project.Calendars.Add("Standard");
Calendar.MakeStandardCalendar(calendar);

project.Set(Prj.Calendar, calendar);

Console.WriteLine("Calendar: " + project.Get(Prj.Calendar).Name);
foreach (var weekDay in calendar.WeekDays)
{
    Console.WriteLine(weekDay.FromDate);
    Console.WriteLine(weekDay.ToDate);
}
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


