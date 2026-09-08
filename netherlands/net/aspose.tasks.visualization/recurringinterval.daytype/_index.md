---
title: "Enum RecurringInterval.DayType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Visualization.RecurringIntervalDayType enum. Vertegenwoordigt een dagtype dat wordt gebruikt in voortgangslijnen"
type: docs
weight: 3320
url: /nl/net/aspose.tasks.visualization/recurringinterval.daytype/
---
## RecurringInterval.DayType enumeration

Vertegenwoordigt een dagtype dat wordt gebruikt in voortgangslijnen.

```csharp
public enum DayType
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Sunday | `1` | Geeft zondag aan. |
| Monday | `2` | Geeft maandag aan. |
| Tuesday | `3` | Geeft dinsdag aan. |
| Wednesday | `4` | Geeft woensdag aan. |
| Thursday | `5` | Geeft donderdag aan. |
| Friday | `6` | Geeft vrijdag aan. |
| Saturday | `7` | Geeft zaterdag aan. |
| Day | `8` | Geeft dag aan. |
| Workday | `9` | Geeft werkdag aan. |
| NonworkingDay | `10` | Geeft niet-werkdag aan. |

## Voorbeelden

Toont hoe te werken met terugkerende intervallen van voortgangslijnen.

```csharp
var project = new Project(DataDir + "Project2007.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[1];

// Laat voortgangslijn lezen.
var interval = view.ProgressLines.RecurringInterval;

Console.WriteLine("Interval: " + interval.Interval);
Console.WriteLine("Weekly Week Number: " + interval.WeeklyWeekNumber);
foreach (var day in interval.WeeklyDays)
{
    Console.WriteLine("Week day: " + day);
}

// Laat terugkerend interval herdefiniëren.
var newInterval = new RecurringInterval();

// Stelt een waarde in die aangeeft of maandelijkse voortgangslijnen per dag moeten worden weergegeven.
interval.MonthlyDay = true;
// Stelt het dagnummer van maandelijkse voortgangslijnen in.
interval.MonthlyDayDayNumber = 1;
// Stelt het maandnummer van maandelijkse voortgangslijnen in.
interval.MonthlyDayMonthNumber = 1;
// Stelt een waarde in die aangeeft of voortgangslijnen moeten worden weergegeven op de eerste of laatste vooraf gedefinieerde dag.
interval.MonthlyFirstLast = true;
// Stelt het type van de eerste of laatste dag van maandelijkse voortgangslijnen in.
interval.MonthlyFirstLastDay = RecurringInterval.DayType.Day;
// Stelt het maandnummer van voortgangslijnen in, die worden weergegeven op de eerste of laatste vooraf gedefinieerde dag.
interval.MonthlyFirstLastMonthNumber = 1;

view.ProgressLines.RecurringInterval = newInterval;

project.Save(OutDir + "WorkWithRecurringInterval_out.pdf", SaveFileFormat.Pdf);
```

### Zie ook

* class [RecurringInterval](../recurringinterval/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


