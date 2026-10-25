---
title: "Classe WeekDayCollection"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.WeekDayCollection. Représente une collection d'objets WeekDay."
type: docs
weight: 3550
url: /fr/net/aspose.tasks/weekdaycollection/
---
## WeekDayCollection class

Représente une collection d'objets [`WeekDay`](../weekday/).

```csharp
public class WeekDayCollection : IList<WeekDay>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../aspose.tasks/weekdaycollection/count/) { get; } | Obtient le nombre d'objets contenus dans cet objet `WeekDayCollection`. |
| [Item](../../aspose.tasks/weekdaycollection/item/) { get; set; } | Obtient ou définit la valeur de l'élément à l'index spécifié. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.tasks/weekdaycollection/add/)(WeekDay) | Ajoute une instance [`WeekDay`](../weekday/) à cet objet. |
| [Clear](../../aspose.tasks/weekdaycollection/clear/)() | Efface l'objet WeekDayCollection. |
| [Contains](../../aspose.tasks/weekdaycollection/contains/)(WeekDay) | Vérifie si la collection contient le [`WeekDay`](../weekday/) spécifié. |
| [CopyTo](../../aspose.tasks/weekdaycollection/copyto/)(WeekDay[], int) | Copie le contenu de la collection dans un tableau à l'index spécifié. |
| [GetEnumerator](../../aspose.tasks/weekdaycollection/getenumerator/)() | Renvoie un énumérateur pour cette collection. |
| [IndexOf](../../aspose.tasks/weekdaycollection/indexof/)(WeekDay) | Renvoie l'index du [`WeekDay`](../weekday/) spécifié. |
| [Insert](../../aspose.tasks/weekdaycollection/insert/)(int, WeekDay) | Insère le [`WeekDay`](../weekday/) à l'index spécifié. |
| [Remove](../../aspose.tasks/weekdaycollection/remove/)(WeekDay) | Supprime le [`WeekDay`](../weekday/) spécifié, le cas échéant. |
| [RemoveAt](../../aspose.tasks/weekdaycollection/removeat/)(int) | Supprime un élément à l'index spécifié. |
| [ToList](../../aspose.tasks/weekdaycollection/tolist/)() | Convertit l'objet WeekDayCollection en une liste d'objets [`WeekDay`](../weekday/). |

## Exemples

Montre comment travailler avec les collections de jours de la semaine.

```csharp
var project = new Project();
var calendar = project.Calendars.GetByName("Standard");

// effacer les jours de la semaine
calendar.WeekDays.Clear();

calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));
var saturday = WeekDay.CreateDefaultWorkingDay(DayType.Saturday);
var sunday = WeekDay.CreateDefaultWorkingDay(DayType.Sunday);

calendar.WeekDays.Add(saturday);
calendar.WeekDays.Add(sunday);

var fridayWorkingTimes = new List<WorkingTime> { new WorkingTime(new DateTime(2020, 4, 13, 8, 0, 0), new DateTime(2020, 4, 13, 12, 0, 0)) };

var friday = new WeekDay(DayType.Friday, fridayWorkingTimes);
if (calendar.WeekDays.Contains(friday))
{
    calendar.WeekDays.Insert(4, friday);
}

Console.WriteLine("Calendar: " + calendar.Name);
Console.WriteLine("Week days count: " + calendar.WeekDays.Count);
foreach (var day in calendar.WeekDays)
{
    Console.WriteLine(day.DayType);
    foreach (var workingTime in day.WorkingTimes)
    {
        Console.WriteLine("From: " + workingTime.From);
        Console.WriteLine("To: " + workingTime.To);
        Console.WriteLine();
    }
}

// supprimer le jour de la semaine samedi
calendar.WeekDays.RemoveAt(5);

// supprimer le jour de la semaine dimanche
if (calendar.WeekDays.IndexOf(saturday) > 0)
{
    calendar.WeekDays.Remove(sunday);
}

Console.WriteLine("Working times after weekend was removed: ");
List<WeekDay> weekDays = calendar.WeekDays.ToList();
foreach (var day in weekDays)
{
    Console.WriteLine(day.DayType);
    foreach (var workingTime in day.WorkingTimes)
    {
        Console.WriteLine("From: " + workingTime.From);
        Console.WriteLine("To: " + workingTime.To);
        Console.WriteLine();
    }
}

var hour24Calendar = project.Calendars.Add("24 Hours");
Calendar.Make24HourCalendar(hour24Calendar);

// copier les jours de la semaine
var weekDaysArray = new WeekDay[calendar.WeekDays.Count];
calendar.WeekDays.CopyTo(weekDaysArray, 0);

foreach (var weekDay in weekDaysArray)
{
    hour24Calendar.WeekDays.Add(weekDay);
}
```

### Voir aussi

* class [WeekDay](../weekday/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


