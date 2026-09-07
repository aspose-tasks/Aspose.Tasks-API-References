---
title: "Classe WeekDayCollection"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.WeekDayCollection. Rappresenta una raccolta di oggetti WeekDay"
type: docs
weight: 3550
url: /it/net/aspose.tasks/weekdaycollection/
---
## WeekDayCollection class

Rappresenta una raccolta di oggetti [`WeekDay`](../weekday/).

```csharp
public class WeekDayCollection : IList<WeekDay>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.tasks/weekdaycollection/count/) { get; } | Ottiene il numero di oggetti contenuti in questo oggetto `WeekDayCollection`. |
| [Item](../../aspose.tasks/weekdaycollection/item/) { get; set; } | Ottiene o imposta il valore dell'elemento all'indice specificato. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.tasks/weekdaycollection/add/)(WeekDay) | Aggiunge un'istanza di [`WeekDay`](../weekday/) a questo oggetto. |
| [Clear](../../aspose.tasks/weekdaycollection/clear/)() | Cancella l'oggetto WeekDayCollection. |
| [Contains](../../aspose.tasks/weekdaycollection/contains/)(WeekDay) | Verifica se la raccolta contiene [`WeekDay`](../weekday/) specificato. |
| [CopyTo](../../aspose.tasks/weekdaycollection/copyto/)(WeekDay[], int) | Copia il contenuto della raccolta in un array all'indice specificato. |
| [GetEnumerator](../../aspose.tasks/weekdaycollection/getenumerator/)() | Restituisce un enumeratore per questa collezione. |
| [IndexOf](../../aspose.tasks/weekdaycollection/indexof/)(WeekDay) | Restituisce l'indice di [`WeekDay`](../weekday/) specificato. |
| [Insert](../../aspose.tasks/weekdaycollection/insert/)(int, WeekDay) | Inserisce [`WeekDay`](../weekday/) all'indice specificato. |
| [Remove](../../aspose.tasks/weekdaycollection/remove/)(WeekDay) | Rimuove [`WeekDay`](../weekday/) specificato, se presente. |
| [RemoveAt](../../aspose.tasks/weekdaycollection/removeat/)(int) | Rimuove un elemento all'indice specificato. |
| [ToList](../../aspose.tasks/weekdaycollection/tolist/)() | Converte l'oggetto WeekDayCollection in un elenco di oggetti [`WeekDay`](../weekday/). |

## Esempi

Mostra come lavorare con le raccolte di giorni della settimana.

```csharp
var project = new Project();
var calendar = project.Calendars.GetByName("Standard");

// cancella i giorni della settimana
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

// rimuovi il giorno della settimana sabato
calendar.WeekDays.RemoveAt(5);

// rimuovi il giorno della settimana domenica
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

// copia i giorni della settimana
var weekDaysArray = new WeekDay[calendar.WeekDays.Count];
calendar.WeekDays.CopyTo(weekDaysArray, 0);

foreach (var weekDay in weekDaysArray)
{
    hour24Calendar.WeekDays.Add(weekDay);
}
```

### Vedi anche

* class [WeekDay](../weekday/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


