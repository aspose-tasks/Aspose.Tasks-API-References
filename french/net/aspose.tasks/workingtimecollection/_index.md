---
title: "Classe WorkingTimeCollection"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.WorkingTimeCollection. Représente une collection d'objets WorkingTimeCollection"
type: docs
weight: 3670
url: /fr/net/aspose.tasks/workingtimecollection/
---
## WorkingTimeCollection class

Représente une collection d'objets `WorkingTimeCollection`.

```csharp
public class WorkingTimeCollection : IList<WorkingTime>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../aspose.tasks/workingtimecollection/count/) { get; } | Obtient le nombre d'objets contenus dans cet objet `WorkingTimeCollection`. |
| [Item](../../aspose.tasks/workingtimecollection/item/) { get; set; } | Renvoie l'élément à l'index spécifié. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.tasks/workingtimecollection/add/)(WorkingTime) | Ajoute une nouvelle instance WorkingTime à cette collection. |
| [Clear](../../aspose.tasks/workingtimecollection/clear/)() | Supprime tous les éléments [`WorkingTime`](../workingtime/) de la collection. |
| [Contains](../../aspose.tasks/workingtimecollection/contains/)(WorkingTime) | Vérifie si l'élément spécifié est dans la List. Effectue une recherche linéaire O(n). |
| [CopyTo](../../aspose.tasks/workingtimecollection/copyto/)(WorkingTime[], int) | Copie le contenu d'une collection dans un Array, en commençant à un indice particulier |
| [GetEnumerator](../../aspose.tasks/workingtimecollection/getenumerator/)() | Renvoie un énumérateur pour cette collection. |
| [Remove](../../aspose.tasks/workingtimecollection/remove/)(WorkingTime) | Supprime l'instance [`WorkingTime`](../workingtime/) de cette collection. |
| [ToList](../../aspose.tasks/workingtimecollection/tolist/)() | Convertit l'objet WorkingTimeCollection en une liste d'objets [`WorkingTime`](../workingtime/). |

## Exemples

Montre comment travailler avec la collection de temps de travail.

```csharp
var project = new Project();
var calendar = project.Calendars.Add("Custom Calendar");

calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));

var saturdayWorkingTimes = new List<WorkingTime>
{
    new WorkingTime(8, 12),
    new WorkingTime(13, 15)
};
var saturday = new WeekDay(DayType.Saturday);
foreach (var time in saturdayWorkingTimes)
{
    saturday.WorkingTimes.Add(time);
}

// imprime les temps de travail du samedi
Console.WriteLine("Saturday working period number: " + saturday.WorkingTimes.Count);
foreach (var time in saturday.WorkingTimes)
{
    Console.WriteLine("From Time: " + time.From);
    Console.WriteLine("To Time: " + time.To);
}

Console.WriteLine();

var sundayWorkingTimes = new List<WorkingTime>
{
    new WorkingTime(10, 15)
};
var sunday = new WeekDay(DayType.Sunday, sundayWorkingTimes);

// imprime les temps de travail du dimanche
List<WorkingTime> workingTimes = sunday.WorkingTimes.ToList();
Console.WriteLine("Sunday working period number: " + workingTimes.Count);
for (var index = 0; index < workingTimes.Count; index++)
{
    var time = workingTimes[index];
    Console.WriteLine("From Time: " + time.From);
    Console.WriteLine("To Time: " + time.To);
}

Console.WriteLine();

calendar.WeekDays.Add(saturday);
calendar.WeekDays.Add(sunday);

foreach (var day in calendar.WeekDays)
{
    Console.WriteLine(day.DayType + ": ");

    // Vous pouvez parcourir davantage les temps de travail et les afficher.
    foreach (var workingTime in day.WorkingTimes)
    {
        Console.WriteLine(workingTime.From);
        Console.WriteLine(workingTime.To);
    }

    Console.WriteLine();
}
```

### Voir aussi

* class [WorkingTime](../workingtime/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


