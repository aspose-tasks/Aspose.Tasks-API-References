---
title: "Calendar.WorkWeeks"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Kalender-eigenschap. Haalt een WorkWeekCollections-object op. De verzameling werkweken die aan de kalender is gekoppeld."
type: docs
weight: 130
url: /nl/net/aspose.tasks/calendar/workweeks/
---
## Calendar.WorkWeeks property

Haalt WorkWeekCollections‑object op. De verzameling werkweken die aan de kalender zijn gekoppeld.

```csharp
public WorkWeekCollection WorkWeeks { get; }
```

## Voorbeelden

Toont hoe werkweekinformatie te lezen.

```csharp
var project = new Project(DataDir + "WorkWithWorkWeekCollection.mpp");
var calendar = project.Calendars.GetByUid(1);

foreach (var workWeek in calendar.WorkWeeks)
{
    // Toon werkweeknaam, van- en totdatums
    var name = workWeek.Name;
    var fromDate = workWeek.FromDate;
    var toDate = workWeek.ToDate;
    Console.WriteLine("Name: " + name);
    Console.WriteLine("From Date: " + fromDate);
    Console.WriteLine("To Date: " + toDate);

    // Deze gegevens gaan over de knop \"Details.\" waarmee je speciale werktijden kunt instellen voor een speciale weekdag of deze zelfs niet-werkend kunt maken
    foreach (var day in workWeek.WeekDays)
    {
        // Je kunt verder door werktijden navigeren en deze weergeven
        foreach (var workingTime in day.WorkingTimes)
        {
            Console.WriteLine(workingTime.From);
            Console.WriteLine(workingTime.To);
        }
    }
}
```

### Zie ook

* class [WorkWeekCollection](../../workweekcollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


