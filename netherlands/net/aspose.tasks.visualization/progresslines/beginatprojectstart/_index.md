---
title: "ProgressLines.BeginAtProjectStart"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ProgressLines eigenschap. Haalt op of stelt een waarde in die aangeeft of voortgangslijnen vanaf het begin van de projectstartdatum moeten worden weergegeven."
type: docs
weight: 30
url: /nl/net/aspose.tasks.visualization/progresslines/beginatprojectstart/
---
## ProgressLines.BeginAtProjectStart property

Haalt een waarde op of stelt deze in die aangeeft of voortgangslijnen moeten worden weergegeven vanaf het begin van de projectstartdatum.

```csharp
public bool BeginAtProjectStart { get; set; }
```

## Voorbeelden

Toont hoe u met voortgangslijnen werkt.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// Laten we een voortgangslijn definiëren.
view.ProgressLines = new ProgressLines();
var progressLines = view.ProgressLines;

// Stel de datum in vanaf wanneer voortgangslijnen worden weergegeven. Laten we de statusdatum van een project instellen.
progressLines.BeginAtDate = project.Get(Prj.StatusDate);
// Stel een waarde in die aangeeft of voortgangslijnen vanaf de begindatum van het project moeten worden weergegeven.
progressLines.BeginAtProjectStart = true;
// Stel het datumformaat in (<see cref="T:Aspose.Tasks.Visualization.DateLabel" />).
progressLines.DateFormat = DateLabel.DayDddd;
// Stel een waarde in die aangeeft of de voortgangslijn op de huidige datum moet worden weergegeven.
progressLines.DisplayAtCurrentDate = true;
// Stel een waarde in die aangeeft of de voortgangslijn op terugkerende intervallen moet worden weergegeven.
progressLines.DisplayAtRecurringIntervals = true;
// Stel een waarde in die aangeeft of voortgangslijnen op de geselecteerde data moeten worden weergegeven.
progressLines.DisplaySelected = true;
// Stel een waarde in die aangeeft of voortgangslijnen voor het baselineschema of de werkelijke waarden moeten worden weergegeven.
progressLines.IsBaselinePlan = false;
// Stel het lettertype in dat wordt gebruikt voor het label van de voortgangslijn.
progressLines.Font = new FontDescriptor("Arial", 10);
// Stel de lijnkleur in voor de huidige voortgangslijn.
progressLines.LineColor = Color.Aquamarine;
// Stel het lijnpatroon in van de huidige voortgangslijn.
progressLines.LinePattern = LinePattern.Dashed;
// Stel de kleur in van andere voortgangslijnen.
progressLines.OtherLineColor = Color.Azure;
// Stel het lijnpatroon in voor andere voortgangslijnen.
progressLines.OtherLinePattern = LinePattern.Dotted;
// Stel de kleur in van andere voortgangspunten.
progressLines.OtherProgressPointColor = Color.Red;
// Stel de vorm van het voortgangspunt in van andere voortgangslijnen.
progressLines.OtherProgressPointShape = GanttBarEndShape.Circle;
// Stel de kleur in van het voortgangspunt.
progressLines.ProgressPointColor = Color.Orange;
// stel de vorm van het voortgangspunt in.
progressLines.ProgressPointShape = GanttBarEndShape.Diamond;
// stel het terugkerende interval in.
progressLines.RecurringInterval = new RecurringInterval();
// stel het terugkerende interval in.
progressLines.RecurringInterval.Interval = Interval.Daily;
// stel het dagelijkse dagnummer in
progressLines.RecurringInterval.DailyDayNumber = 1;
// stel een waarde in die aangeeft of de datum voor elke voortgangslijn moet worden weergegeven.
progressLines.ShowDate = true;

// laten we voortgangslijnen controleren
Console.WriteLine("Begin At Date: " + progressLines.BeginAtDate);
Console.WriteLine("Begin At Project Start: " + progressLines.BeginAtProjectStart);
Console.WriteLine("Date Format: " + progressLines.DateFormat);
Console.WriteLine("Display At Current Date: " + progressLines.DisplayAtCurrentDate);
Console.WriteLine("Display At Recurring Intervals: " + progressLines.DisplayAtRecurringIntervals);
Console.WriteLine("Display Selected: " + progressLines.DisplaySelected);
Console.WriteLine("Font: " + progressLines.Font);
Console.WriteLine("Is Baseline Plan: " + progressLines.IsBaselinePlan);
Console.WriteLine("Line Color: " + progressLines.LineColor);
Console.WriteLine("Line Pattern: " + progressLines.LinePattern);
Console.WriteLine("Other Line Color: " + progressLines.OtherLineColor);
Console.WriteLine("Other Line Pattern: " + progressLines.OtherLinePattern);
Console.WriteLine("Other Progress Point Color: " + progressLines.OtherProgressPointColor);
Console.WriteLine("Other Progress Point Shape: " + progressLines.OtherProgressPointShape);
Console.WriteLine("Progress Point Color: " + progressLines.ProgressPointColor);
Console.WriteLine("Progress Point Shape: " + progressLines.ProgressPointShape);
Console.WriteLine("Recurring Interval: " + progressLines.RecurringInterval.Interval);
Console.WriteLine("Recurring Interval DailyDayNumber: " + progressLines.RecurringInterval.DailyDayNumber);
Console.WriteLine("Selected Dates: ");
foreach (var date in progressLines.SelectedDates)
{
    Console.WriteLine("Date: " + date);
}
Console.WriteLine("Show Date: " + progressLines.ShowDate);
Console.WriteLine();

project.Save(OutDir + "WorkWithProgressLines_out.mpp", SaveFileFormat.Mpp);
```

### Zie ook

* class [ProgressLines](../)
* namespace [Aspose.Tasks.Visualization](../../progresslines/)
* assembly [Aspose.Tasks](../../../)


