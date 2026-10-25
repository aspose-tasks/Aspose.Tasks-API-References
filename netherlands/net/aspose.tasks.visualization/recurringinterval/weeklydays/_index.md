---
title: "RecurringInterval.WeeklyDays"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "RecurringInterval eigenschap. Haalt een lijst met dagen op voor wekelijkse voortgangslijnen."
type: docs
weight: 110
url: /nl/net/aspose.tasks.visualization/recurringinterval/weeklydays/
---
## RecurringInterval.WeeklyDays property

Haalt een lijst met dagen op voor wekelijkse voortgangslijnen.

```csharp
public List<DayType> WeeklyDays { get; }
```

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

* enum [DayType](../../recurringinterval.daytype/)
* class [RecurringInterval](../)
* namespace [Aspose.Tasks.Visualization](../../recurringinterval/)
* assembly [Aspose.Tasks](../../../)


