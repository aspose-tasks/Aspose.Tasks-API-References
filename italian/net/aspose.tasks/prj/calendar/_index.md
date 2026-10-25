---
title: "Prj.Calendar"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. Il calendario del progetto"
type: docs
weight: 90
url: /it/net/aspose.tasks/prj/calendar/
---
## Prj.Calendar field

Il calendario del progetto.

```csharp
public static readonly Key<Calendar, PrjKey> Calendar;
```

## Esempi

Mostra come leggere/scrivere la proprietà Prj.Calendar.

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

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


