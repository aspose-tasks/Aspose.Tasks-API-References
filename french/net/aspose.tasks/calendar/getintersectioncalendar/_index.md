---
title: "Calendar.GetIntersectionCalendar"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Calendar. Obtient une instance ICalendar qui peut être utilisée pour effectuer des calculs sur l'intersection des horaires de travail de 2 calendriers"
type: docs
weight: 280
url: /fr/net/aspose.tasks/calendar/getintersectioncalendar/
---
## Calendar.GetIntersectionCalendar method

Obtient l'instance [`ICalendar`](../../icalendar/) qui peut être utilisée pour effectuer des calculs sur l'intersection des horaires de travail de 2 calendriers.

```csharp
public static ICalendar GetIntersectionCalendar(Calendar calendar1, Calendar calendar2)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| calendar1 | Calendar | Premier calendrier. |
| calendar2 | Calendar | Deuxième calendrier. |

### Valeur de retour

Implémentation de l'interface ICalendar.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | Lorsque l'un des arguments est nul. |

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

* interface [ICalendar](../../icalendar/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


