---
title: "Classe DayTypeCollection"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.DayTypeCollection. Représente une collection d'objets DayType"
type: docs
weight: 460
url: /fr/net/aspose.tasks/daytypecollection/
---
## DayTypeCollection class

Représente une collection d'objets [`DayType`](../daytype/).

```csharp
public class DayTypeCollection : IList<DayType>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../aspose.tasks/daytypecollection/count/) { get; } | Obtient le nombre d'éléments contenus dans cette collection. |
| [IsReadOnly](../../aspose.tasks/daytypecollection/isreadonly/) { get; } | Obtient une valeur indiquant si cette collection est en lecture seule ; sinon, false. |
| [Item](../../aspose.tasks/daytypecollection/item/) { get; set; } | Renvoie ou définit l'élément à l'index spécifié. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.tasks/daytypecollection/add/)(DayType) | Ajoute l'élément spécifié à cette collection. |
| [Clear](../../aspose.tasks/daytypecollection/clear/)() | Supprime tous les éléments de cette collection. |
| [Contains](../../aspose.tasks/daytypecollection/contains/)(DayType) | Renvoie true si l'élément spécifié est trouvé dans cette collection ; sinon, false. |
| [CopyTo](../../aspose.tasks/daytypecollection/copyto/)(DayType[], int) | Copie les éléments de cette collection dans le tableau spécifié, en commençant à l'index de tableau spécifié. |
| [GetEnumerator](../../aspose.tasks/daytypecollection/getenumerator/)() | Renvoie un énumérateur pour cette collection. |
| [IndexOf](../../aspose.tasks/daytypecollection/indexof/)(DayType) | Détermine l'index de l'élément spécifié dans cette collection. |
| [Insert](../../aspose.tasks/daytypecollection/insert/)(int, DayType) | Insère l'élément spécifié à l'index spécifié. |
| [Remove](../../aspose.tasks/daytypecollection/remove/)(DayType) | Supprime la première occurrence d'un objet spécifique de cette collection. |
| [RemoveAt](../../aspose.tasks/daytypecollection/removeat/)(int) | Supprime un élément à l'index spécifié. |

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

* enum [DayType](../daytype/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


