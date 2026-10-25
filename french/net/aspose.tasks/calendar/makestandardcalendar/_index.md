---
title: "Calendar.MakeStandardCalendar"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Calendar. Crée un calendrier standard par défaut"
type: docs
weight: 30
url: /fr/net/aspose.tasks/calendar/makestandardcalendar/
---
## Calendar.MakeStandardCalendar method

Crée un calendrier standard par défaut.

```csharp
public static Calendar MakeStandardCalendar(Calendar calendar)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| calendrier | Calendar | Calendrier à partir duquel créer un calendrier standard. |

### Valeur de retour

Calendrier avec 5 jours ouvrés (lundi-vendredi) avec des horaires de travail de 8-12 et 13-17.

## Exemples

Montre comment créer un calendrier standard.

```csharp
Project project = new Project();
var calendar = project.Calendars.Add("New calendar");
Calendar.MakeStandardCalendar(calendar);

var workingHours = calendar.GetWorkingTimes(new DateTime(2020, 4, 8));

// afficher les heures de travail
foreach (var wh in workingHours)
{
    Console.WriteLine("From: " + wh.From);
    Console.WriteLine("To: " + wh.To);
}
```

Montre comment créer un calendrier avec des jours d'exception.

```csharp
var project = new Project(DataDir + "project_update_test.mpp");
var calendar = project.Calendars.GetByName("Standard");

// Mettre à jour les informations du calendrier
Calendar.MakeStandardCalendar(calendar);
calendar.Name = "Test calendar";
var exception = new CalendarException();
exception.Name = "Exception 1";
exception.FromDate = DateTime.Now;
exception.ToDate = DateTime.Now.AddDays(2);
exception.DayWorking = true;

exception.WorkingTimes.Add(new WorkingTime(9, 13));
exception.WorkingTimes.Add(new WorkingTime(14, 19));
exception.WorkingTimes.Add(new WorkingTime(20, 21));
calendar.Exceptions.Add(exception);

var exception2 = new CalendarException();
exception.Name = "Exception 2";
exception2.FromDate = DateTime.Now.AddDays(7);
exception2.ToDate = exception2.FromDate;
exception2.DayWorking = false;
calendar.Exceptions.Add(exception2);

project.Set(Prj.Calendar, calendar);

project.Save(OutDir + "WriteUpdatedCalendarDataToMPP_out.mpp", SaveFileFormat.Mpp);
```

### Voir aussi

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


