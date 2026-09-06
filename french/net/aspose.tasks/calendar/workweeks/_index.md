---
title: "Calendar.WorkWeeks"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Calendar. Obtient l'objet WorkWeekCollections. La collection de semaines de travail associée au calendrier."
type: docs
weight: 130
url: /fr/net/aspose.tasks/calendar/workweeks/
---
## Calendar.WorkWeeks property

Obtient l'objet WorkWeekCollections. La collection des semaines de travail associée au calendrier.

```csharp
public WorkWeekCollection WorkWeeks { get; }
```

## Exemples

Montre comment lire les informations des semaines de travail.

```csharp
var project = new Project(DataDir + "WorkWithWorkWeekCollection.mpp");
var calendar = project.Calendars.GetByUid(1);

foreach (var workWeek in calendar.WorkWeeks)
{
    // Afficher le nom de la semaine de travail, les dates de début et de fin
    var name = workWeek.Name;
    var fromDate = workWeek.FromDate;
    var toDate = workWeek.ToDate;
    Console.WriteLine("Name: " + name);
    Console.WriteLine("From Date: " + fromDate);
    Console.WriteLine("To Date: " + toDate);

    // Ces données concernent le bouton \"Détails.\" vous pouvez définir des temps de travail spéciaux pour un jour de semaine spécial ou même le rendre non ouvrable.
    foreach (var day in workWeek.WeekDays)
    {
        // Vous pouvez parcourir davantage les temps de travail et les afficher.
        foreach (var workingTime in day.WorkingTimes)
        {
            Console.WriteLine(workingTime.From);
            Console.WriteLine(workingTime.To);
        }
    }
}
```

### Voir aussi

* class [WorkWeekCollection](../../workweekcollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


