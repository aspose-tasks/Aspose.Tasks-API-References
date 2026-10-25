---
title: "Klasse RecurringInterval"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Visualization.RecurringInterval klasse. Vertegenwoordigt terugkerende intervallen die worden gebruikt in voortgangslijnen van een Gantt‑diagramweergave"
type: docs
weight: 3310
url: /nl/net/aspose.tasks.visualization/recurringinterval/
---
## RecurringInterval class

Stelt terugkerende intervallen voor die worden gebruikt in voortgangslijnen van een Gantt‑diagramweergave.

```csharp
public class RecurringInterval
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [RecurringInterval](recurringinterval/)() | De standaardconstructor. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [DailyDayNumber](../../aspose.tasks.visualization/recurringinterval/dailydaynumber/) { get; set; } | Haalt of stelt het dagelijkse dagnummer in. |
| [DailyWorkday](../../aspose.tasks.visualization/recurringinterval/dailyworkday/) { get; set; } | Haalt of stelt een waarde in die aangeeft of een dag een werkdag is voor dagelijkse voortgangslijnen. |
| [Interval](../../aspose.tasks.visualization/recurringinterval/interval/) { get; set; } | Haalt of stelt het terugkerende interval in. Kan elke waarde van het type [`Interval`](./interval/) zijn. |
| [MonthlyDay](../../aspose.tasks.visualization/recurringinterval/monthlyday/) { get; set; } | Haalt of stelt een waarde in die aangeeft of maandelijkse voortgangslijnen per dag moeten worden weergegeven. |
| [MonthlyDayDayNumber](../../aspose.tasks.visualization/recurringinterval/monthlydaydaynumber/) { get; set; } | Haalt of stelt het dagnummer van maandelijkse voortgangslijnen in. |
| [MonthlyDayMonthNumber](../../aspose.tasks.visualization/recurringinterval/monthlydaymonthnumber/) { get; set; } | Haalt of stelt het maandnummer van maandelijkse voortgangslijnen in. |
| [MonthlyFirstLast](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlast/) { get; set; } | Haalt of stelt een waarde in die aangeeft of voortgangslijnen moeten worden weergegeven op basis van de eerste of laatste vooraf gedefinieerde dag. |
| [MonthlyFirstLastDay](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlastday/) { get; set; } | Haalt of stelt het type van de eerste of laatste dag van maandelijkse voortgangslijnen in. |
| [MonthlyFirstLastMonthNumber](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlastmonthnumber/) { get; set; } | Haalt of stelt het maandnummer van voortgangslijnen in, die worden weergegeven op basis van de eerste of laatste vooraf gedefinieerde dag. |
| [WeeklyDays](../../aspose.tasks.visualization/recurringinterval/weeklydays/) { get; } | Haalt een lijst met dagen op voor wekelijkse voortgangslijnen. |
| [WeeklyWeekNumber](../../aspose.tasks.visualization/recurringinterval/weeklyweeknumber/) { get; set; } | Haalt of stelt het weeknummer voor wekelijkse voortgangslijnen in. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


