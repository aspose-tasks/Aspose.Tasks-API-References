---
title: "Calendar.MakeNightShiftCalendar"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Calendar. Transforme un Calendar donné en Night Shift Calendar"
type: docs
weight: 20
url: /fr/net/aspose.tasks/calendar/makenightshiftcalendar/
---
## Calendar.MakeNightShiftCalendar method

Transforme un calendrier donné en calendrier de quart de nuit.

```csharp
public static Calendar MakeNightShiftCalendar(Calendar calendar)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| calendrier | Calendar | Calendar pour créer Night Shift Calendar. |

### Valeur de retour

Night Shift Calendar.

## Exemples

Montre comment créer un Night Shift Calendar.

```csharp
Project project = new Project();
var calendar = project.Calendars.Add("New calendar");
Calendar.MakeNightShiftCalendar(calendar);

var workingHours = calendar.GetWorkingTimes(new DateTime(2020, 4, 8));

// afficher les heures de travail
foreach (var wh in workingHours)
{
    Console.WriteLine("From: " + wh.From);
    Console.WriteLine("To: " + wh.To);
}
```

Montre comment transformer un calendrier en Night Shift Calendar.

```csharp
var project = new Project();

var calendar = project.Calendars.Add("Night Shift");
calendar = Calendar.MakeNightShiftCalendar(calendar);

var workingHours = calendar.GetWorkingTimes(new DateTime(2020, 4, 8));

// afficher les heures de travail
foreach (var wh in workingHours)
{
    Console.WriteLine("From: " + wh.From);
    Console.WriteLine("To: " + wh.To);
}
```

### Voir aussi

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


