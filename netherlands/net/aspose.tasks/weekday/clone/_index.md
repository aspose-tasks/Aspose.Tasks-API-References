---
title: "WeekDay.Clone"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "WeekDay-methode. Retourneert een diepe kopie van de weekdag"
type: docs
weight: 80
url: /nl/net/aspose.tasks/weekday/clone/
---
## WeekDay.Clone method

Retourneert een diepe kopie van de weekdag.

```csharp
public WeekDay Clone()
```

### Retourwaarde

Retourneert de diepe kopie van de weekdag.

## Voorbeelden

Toont hoe een weekdag te klonen.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var calendar = project.Calendars.GetByUid(1);
var weekDay1 = calendar.WeekDays[0];

// maak een diepe kopie van een weekdag
var weekDay2 = weekDay1.Clone();

// de gelijkheid van kalenders wordt gecontroleerd aan de hand van de eigenschappen van de weekdag:
// weekday.DayType
// weekday.DayWorking
// weekday.FromDate
// weekday.ToDate
// weekday.WorkingTimes
Console.WriteLine("WeekDay 1 Day Type: " + weekDay1.DayType);
Console.WriteLine("WeekDay 1 Day Working: " + weekDay1.DayWorking);
Console.WriteLine("WeekDay 1 From Date: " + weekDay1.FromDate);
Console.WriteLine("WeekDay 1 From Date: " + weekDay1.ToDate);
Console.WriteLine("WeekDay 1 WorkingTimes: " + weekDay1.WorkingTimes);
Console.WriteLine("WeekDay 2 Day Type: " + weekDay2.DayType);
Console.WriteLine("WeekDay 2 Day Working: " + weekDay2.DayWorking);
Console.WriteLine("WeekDay 2 From Date: " + weekDay2.FromDate);
Console.WriteLine("WeekDay 2 From Date: " + weekDay2.ToDate);
Console.WriteLine("WeekDay 2 WorkingTimes: " + weekDay2.WorkingTimes);
Console.WriteLine("Are weekdays equal: " + weekDay1.Equals(weekDay2));
Console.WriteLine("Are weekdays equal (by reference): " + ReferenceEquals(weekDay1, weekDay2));
```

### Zie ook

* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)


