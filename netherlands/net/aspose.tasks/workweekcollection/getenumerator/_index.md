---
title: "WorkWeekCollection.GetEnumerator"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "WorkWeekCollection-methode. Retourneert een enumerator voor deze collectie"
type: docs
weight: 50
url: /nl/net/aspose.tasks/workweekcollection/getenumerator/
---
## WorkWeekCollection.GetEnumerator method

Retourneert een enumerator voor deze collectie.

```csharp
public IEnumerator<WorkWeek> GetEnumerator()
```

### Retourwaarde

een enumerator voor deze collectie.

## Voorbeelden

Toont hoe u een aangepaste werkweek voor een agenda maakt.

```csharp
var project = new Project();
var calendar = project.Calendars.Add("Standard");
Calendar.MakeStandardCalendar(calendar);

var item = new WorkWeek();
item.Name = "My Work Week";
item.FromDate = new DateTime(2020, 4, 13, 8, 0, 0);
item.ToDate = new DateTime(2020, 4, 17, 17, 0, 0);
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));
item.WeekDays.Add(new WeekDay(DayType.Saturday));
item.WeekDays.Add(new WeekDay(DayType.Sunday));
calendar.WorkWeeks.Add(item);

Console.WriteLine("Work Weeks Count: " + calendar.WorkWeeks.Count);
foreach (var workWeek in calendar.WorkWeeks)
{
    // Toon de naam van de werkweek, de naam van de bovenliggende kalender, van‑ en tot‑datums.
    Console.WriteLine("Name: " + workWeek.Name);
    Console.WriteLine("Parent calendar name: " + calendar.Name);
    Console.WriteLine("From Date: " + workWeek.FromDate);
    Console.WriteLine("To Date: " + workWeek.ToDate);
    Console.WriteLine();

    // Deze gegevens gaan over de knop \"Details.\" waarmee je speciale werktijden kunt instellen voor een speciale weekdag of deze zelfs niet-werkend kunt maken
    List<WeekDay> weekDays = workWeek.WeekDays.ToList();
    foreach (var day in weekDays)
    {
        Console.WriteLine(day.DayType.ToString());

        // Je kunt verder door werktijden navigeren en deze weergeven
        foreach (var workingTime in day.WorkingTimes)
        {
            Console.WriteLine(workingTime.From);
            Console.WriteLine(workingTime.To);
        }
    }

    Console.WriteLine();
}
```

### Zie ook

* class [WorkWeek](../../workweek/)
* class [WorkWeekCollection](../)
* namespace [Aspose.Tasks](../../workweekcollection/)
* assembly [Aspose.Tasks](../../../)


