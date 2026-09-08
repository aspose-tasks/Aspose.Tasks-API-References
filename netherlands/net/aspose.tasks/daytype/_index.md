---
title: "Enum DayType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.DayType enum. Specificeert de dag van de week"
type: docs
weight: 450
url: /nl/net/aspose.tasks/daytype/
---
## DayType enumeration

Specificeert de dag van een week.

```csharp
public enum DayType
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Exception | `0` | Geeft het type dag Exception aan. |
| Sunday | `1` | Geeft het type dag Sunday aan. |
| Monday | `2` | Geeft het type dag Monday aan. |
| Tuesday | `3` | Geeft het type dag Tuesday aan. |
| Wednesday | `4` | Geeft het type dag Wednesday aan. |
| Thursday | `5` | Geeft het type dag Thursday aan. |
| Friday | `6` | Geeft het type dag Friday aan. |
| Saturday | `7` | Geeft het type dag Saturday aan. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


