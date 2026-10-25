---
title: "ICalendar.GetWorkingTimes"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ICalendar. Retourne WorkingTimeCollection des créneaux de travail pour la date spécifiée."
type: docs
weight: 80
url: /fr/net/aspose.tasks/icalendar/getworkingtimes/
---
## ICalendar.GetWorkingTimes method

Retourne [`WorkingTimeCollection`](../../workingtimecollection/) des créneaux de travail pour la date spécifiée.

```csharp
public WorkingTimeCollection GetWorkingTimes(DateTime dt)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| dt | DateTime | La date pour laquelle obtenir les heures de travail. |

### Valeur de retour

Collection d'instances de [`WorkingTime`](../../workingtime/).

## Exemples

Montre comment utiliser la méthode Calendar.GetIntersectionCalendar() pour effectuer le calcul sur le calendrier de l'affectation.

```csharp
var project = new Project(DataDir + "CalculateWorkHours.mpp");

foreach (var ra in project.ResourceAssignments)
{
    if (ra.Resource == null)
    {
        continue;
    }

    ICalendar assignmentCalendar;

    Calendar taskCalendar = ra.Task.Calendar != null && !ra.Task.Duration.IsEstimated ? ra.Task.Calendar : null;
    Calendar resourceCalendar = ra.Resource.Calendar != null && !ra.Task.IgnoreResourceCalendar
        ? ra.Resource.Calendar
        : null;

    if (taskCalendar != null && resourceCalendar != null && !ReferenceEquals(taskCalendar, resourceCalendar))
    {
        assignmentCalendar = Calendar.GetIntersectionCalendar(taskCalendar, resourceCalendar);
    }
    else
    {
        assignmentCalendar = taskCalendar ?? resourceCalendar;
    }

    if (assignmentCalendar == null)
    {
        assignmentCalendar = project.Calendar;
    }

    var workingHours = assignmentCalendar.GetWorkingHours(ra.Start, ra.Finish);

    Console.WriteLine("Working hours for assignment '{0}' : {1}", ra, workingHours);

    var date = new DateTime(2025, 4, 7);
    Console.WriteLine("Working times for date '{0}':", date);

    foreach (var wt in assignmentCalendar.GetWorkingTimes(date))
    {
        Console.WriteLine("{0} - {1}", wt.From.TimeOfDay, wt.To.TimeOfDay);
    }
}
```

### Voir aussi

* class [WorkingTimeCollection](../../workingtimecollection/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


