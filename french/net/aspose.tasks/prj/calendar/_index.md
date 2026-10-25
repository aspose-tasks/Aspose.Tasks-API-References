---
title: "Prj.Calendar"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Le calendrier du projet"
type: docs
weight: 90
url: /fr/net/aspose.tasks/prj/calendar/
---
## Prj.Calendar field

Le calendrier du projet.

```csharp
public static readonly Key<Calendar, PrjKey> Calendar;
```

## Exemples

Montre comment lire/écrire la propriété Prj.Calendar.

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

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


