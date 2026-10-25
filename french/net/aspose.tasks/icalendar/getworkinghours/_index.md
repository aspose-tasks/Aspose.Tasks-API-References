---
title: "ICalendar.GetWorkingHours"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ICalendar. Retourne le WorkUnit  Début Fin et Durée des heures de travail pour l'intervalle de date et d'heure spécifié."
type: docs
weight: 60
url: /fr/net/aspose.tasks/icalendar/getworkinghours/
---
## GetWorkingHours(DateTime, DateTime) {#getworkinghours}

Renvoie WorkUnit - Début, Fin et Durée des heures de travail pour l'intervalle de date et d'heure spécifié.

```csharp
public WorkUnit GetWorkingHours(DateTime start, DateTime finish)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| début | DateTime | Date de début de l'intervalle. |
| fin | DateTime | Date de fin de l'intervalle. |

### Valeur de retour

Instance de la classe [`WorkUnit`](../../workunit/) contenant le Début, la Fin et la Durée des heures de travail.

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

* class [WorkUnit](../../workunit/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetWorkingHours(DateTime) {#getworkinghours_1}

Renvoie le nombre d'heures de travail à la date spécifiée.

```csharp
public TimeSpan GetWorkingHours(DateTime dt)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| dt | DateTime | La date pour laquelle obtenir les heures de travail. |

### Valeur de retour

Heures de travail à la date spécifiée.

### Voir aussi

* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


