---
title: "TimelineView.ShowPanZoom"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TimelineView eigenschap. Haalt een waarde op of stelt deze in die aangeeft of de pan‑ en zoombediening moet worden weergegeven."
type: docs
weight: 50
url: /nl/net/aspose.tasks/timelineview/showpanzoom/
---
## TimelineView.ShowPanZoom property

Haalt een waarde op of stelt een waarde in die aangeeft of pan- en zoombesturing worden weergegeven.

```csharp
public bool ShowPanZoom { get; set; }
```

## Voorbeelden

Toont hoe te werken met &lt;see cref="Aspose.Tasks.TimelineView" /&gt;.

```csharp
var project = new Project();

// initialiseer een tijdlijnweergave
var view = new TimelineView();

// stel een waarde in die aangeeft hoe datums op de tijdlijnweergave worden opgemaakt.
view.DateFormat = DateFormat.DateDddDd;
// stel een waarde in die aangeeft of overlappende taken op meerdere rijen worden weergegeven.
view.DisplayOverlapped = true;
// stel een waarde in die aangeeft of pan- en zoombesturing worden weergegeven.
view.ShowPanZoom = true;
// stel een waarde in die aangeeft of de tijdschaal wordt weergegeven.
view.ShowTimescale = true;
// stel een waarde in die aangeeft of een lijn die vandaag representeert, wordt weergegeven.
view.ShowToday = true;
// stel een waarde in die aangeeft hoeveel lijnen worden gebruikt om taken in een tijdlijn weer te geven.
view.TextLinesCount = 2;

// haalt een waarde op die aangeeft of overlappende taken op meerdere rijen worden weergegeven.
Console.WriteLine("Show Dates: " + view.ShowDates);

// voeg de weergave toe aan het project
project.Views.Add(view);

// voeg wat testgegevens toe aan het project
var task1 = project.RootTask.Children.Add("Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 4, 29, 8, 0, 0));
task1.Set(Tsk.Duration, task1.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Start, new DateTime(2020, 4, 29, 8, 0, 0));
task2.Set(Tsk.Duration, task1.ParentProject.GetDuration(40, TimeUnitType.Hour));

project.Save(OutDir + "SetTimeScaleCount_out.pdf", SaveFileFormat.Pdf);
```

### Zie ook

* class [TimelineView](../)
* namespace [Aspose.Tasks](../../timelineview/)
* assembly [Aspose.Tasks](../../../)


