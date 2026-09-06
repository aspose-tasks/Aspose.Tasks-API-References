---
title: "DayTypeCollection.Remove"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "DayTypeCollection méthode. Supprime la première occurrence d'un objet spécifique de cette collection"
type: docs
weight: 110
url: /fr/net/aspose.tasks/daytypecollection/remove/
---
## DayTypeCollection.Remove method

Supprime la première occurrence d'un objet spécifique de cette collection.

```csharp
public bool Remove(DayType item)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| élément | DayType | l'objet spécifié à supprimer. |

### Valeur de retour

true si l'objet spécifié a été supprimé avec succès de cette collection ; sinon, false.

## Exemples

Montre comment utiliser une collection de jours de la semaine pour définir une exception de calendrier hebdomadaire.

```csharp
var project = new Project(DataDir + "WeeklyDayTypeException.mpp");
var calendar = project.Calendars.GetByUid(1);

foreach (var calendarException in calendar.Exceptions)
{
    Console.WriteLine("Exception Name: " + calendarException.Name);
    Console.WriteLine("Days of week count: " + calendarException.DaysOfWeek.Count);
    foreach (var dayType in calendarException.DaysOfWeek)
    {
        Console.WriteLine("Day type: " + dayType);
    }

    Console.WriteLine();
}

var exc1 = calendar.Exceptions.ToList()[0];
if (!exc1.DaysOfWeek.IsReadOnly && exc1.DaysOfWeek.IndexOf(DayType.Monday) < 0)
{
    exc1.DaysOfWeek.Insert(0, DayType.Wednesday);
}

var exc2 = calendar.Exceptions.ToList()[1];
if (exc2.DaysOfWeek.Contains(DayType.Sunday))
{
    // supprimer un type de jour de "Exception 2" par type de jour
    exc2.DaysOfWeek.Remove(DayType.Sunday);
}

// supprimer un type de jour de "Exception 2" par indice
Console.WriteLine("Remove " + exc2.DaysOfWeek[0] + " day type from exception by index...");
exc2.DaysOfWeek.RemoveAt(0);

// Modifier les exceptions (il n'y a aucune exception dans les données du projet initial)
var exc4 = new CalendarException
               {
                   Name = "Weekly Exception 2",
                   FromDate = new DateTime(2020, 4, 13),
                   ToDate = new DateTime(2020, 4, 18),
                   Occurrences = 3,
                   Type = CalendarExceptionType.Weekly
               };
exc4.DaysOfWeek.Add(DayType.Monday);
exc4.DaysOfWeek.Add(DayType.Thursday);

calendar.Exceptions.Add(exc4);

var exc3 = calendar.Exceptions.ToList()[2];

// supprimer tous les jours de la semaine pour "Exception 3"
exc3.DaysOfWeek.Clear();

var dayTypes = new DayType[exc4.DaysOfWeek.Count];
exc4.DaysOfWeek.CopyTo(dayTypes, 0);

foreach (var dayType in dayTypes)
{
    exc3.DaysOfWeek.Add(dayType);
}

Console.WriteLine("Days of week for exception: " + exc3.Name);
foreach (var dayType in exc3.DaysOfWeek)
{
    Console.WriteLine("Day type: " + dayType);
}
```

### Voir aussi

* enum [DayType](../../daytype/)
* class [DayTypeCollection](../)
* namespace [Aspose.Tasks](../../daytypecollection/)
* assembly [Aspose.Tasks](../../../)


