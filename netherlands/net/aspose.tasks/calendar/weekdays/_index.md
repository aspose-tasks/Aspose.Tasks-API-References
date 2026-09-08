---
title: "Calendar.WeekDays"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Calendar-eigenschap. Haalt een WeekDaysCollection op voor deze kalender. De verzameling weekdagen die de kalender definieert"
type: docs
weight: 120
url: /nl/net/aspose.tasks/calendar/weekdays/
---
## Calendar.WeekDays property

Haalt WeekDaysCollection op voor deze kalender. De verzameling weekdagen die de kalender definieert.

```csharp
public WeekDayCollection WeekDays { get; }
```

## Voorbeelden

Toont hoe je een nieuwe kalender definieert, weekdagen toevoegt en werktijden voor dagen definieert.

```csharp
var project = new Project();

// Definieer een kalender
var calendar = project.Calendars.Add("Calendar1");

// Voeg werkdagen toe van maandag tot en met donderdag met standaardtijden
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// Stel vrijdag in als korte werkdag
var weekDay = new WeekDay(DayType.Friday);

// Stelt werktijd in. Alleen het tijdgedeelte van DateTime is belangrijk.
var workingTime = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 16);
weekDay.WorkingTimes.Add(workingTime);
weekDay.WorkingTimes.Add(workingTime2);
weekDay.DayWorking = true;
calendar.WeekDays.Add(weekDay);

// werken met het project...
```

### Zie ook

* class [WeekDayCollection](../../weekdaycollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


