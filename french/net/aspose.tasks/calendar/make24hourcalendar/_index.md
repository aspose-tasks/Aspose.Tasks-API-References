---
title: "Calendar.Make24HourCalendar"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Calendar. Transforme un calendrier donné en calendrier 24 heures. Un calendrier 24 heures est un calendrier où chaque jour de la semaine travaille avec des heures de travail en continu."
type: docs
weight: 10
url: /fr/net/aspose.tasks/calendar/make24hourcalendar/
---
## Calendar.Make24HourCalendar method

Transforme un calendrier donné en calendrier 24Heures. Le calendrier 24Heures est un calendrier dans lequel chaque jour de la semaine travaille avec des heures de travail 24/24.

```csharp
public static Calendar Make24HourCalendar(Calendar calendar)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| calendrier | Calendar | Calendrier pour créer un calendrier de 24 heures à partir de. |

### Valeur de retour

Calendrier 24 heures.

## Exemples

Montre comment créer un calendrier de 24 heures.

```csharp
Project project = new Project();
var calendar = project.Calendars.Add("New calendar");
Calendar.Make24HourCalendar(calendar);

var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0));

// 24 heures seront imprimées
Console.WriteLine("Hours: " + workingHours.TotalHours);
```

Montre comment transformer un nouveau calendrier en un calendrier de 24 heures.

```csharp
var project = new Project();

var calendar = project.Calendars.Add("24 Hours");
calendar = Calendar.Make24HourCalendar(calendar);

var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0));

// 24 heures seront imprimées
Console.WriteLine("Hours: " + workingHours.TotalHours);
```

### Voir aussi

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


