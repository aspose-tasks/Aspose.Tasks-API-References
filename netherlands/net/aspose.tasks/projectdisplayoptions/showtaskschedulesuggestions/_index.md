---
title: "ProjectDisplayOptions.ShowTaskScheduleSuggestions"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ProjectDisplayOptions property. Haalt op of stelt een waarde in die aangeeft of suggesties moeten worden getoond wanneer Project een mogelijk planningsconflict detecteert met een handmatig geplande taak. Deze optie is beschikbaar voor Project 2010 en latere versies"
type: docs
weight: 80
url: /nl/net/aspose.tasks/projectdisplayoptions/showtaskschedulesuggestions/
---
## ProjectDisplayOptions.ShowTaskScheduleSuggestions property

Haalt op of stelt een waarde in die aangeeft of suggesties moeten worden getoond wanneer Project een mogelijk planningsconflict identificeert met een handmatig geplande taak. Deze optie is beschikbaar voor Project 2010 en latere versies.

```csharp
public bool ShowTaskScheduleSuggestions { get; set; }
```

## Voorbeelden

Toont hoe de weergave‑opties van het project te gebruiken.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// Stel een waarde in die aangeeft of waarschuwingen moeten worden weergegeven wanneer Project een mogelijk planningsconflict detecteert met een handmatig ingeplande taak.
// Deze optie is beschikbaar voor Project 2010 en later.
project.DisplayOptions.ShowTaskScheduleWarnings = false;

// een waarde die aangeeft of er een spatie moet worden toegevoegd vóór de numerieke waarde en de tijdsaanduiding (1 wk in plaats van 1wk)
project.DisplayOptions.AddSpaceBeforeLabel = true;

// stel in hoe het minutenlabel wordt weergegeven
project.DisplayOptions.MinuteLabel = MinuteLabelDisplay.Min;

// stel in hoe het uurlabel wordt weergegeven
project.DisplayOptions.HourLabel = HourLabelDisplay.Hr;

// stel in hoe het daglabel wordt weergegeven
project.DisplayOptions.DayLabel = DayLabelDisplay.Dy;

// stel in hoe het weeklabel wordt weergegeven
project.DisplayOptions.WeekLabel = WeekLabelDisplay.Week;

// stel in hoe het maandlabel wordt weergegeven
project.DisplayOptions.MonthLabel = MonthLabelDisplay.Mon;

// Stel in hoe het jaartitel wordt weergegeven
project.DisplayOptions.YearLabel = YearLabelDisplay.Year;

// stel een waarde in die aangeeft of samenvattende informatie over een heel project op één rij moet worden weergegeven met een eigen samenvattende taakbalk bovenaan de Gantt‑chartweergave.
project.DisplayOptions.ShowProjectSummaryTask = true;

// stel een waarde in die aangeeft of suggesties moeten worden getoond wanneer Project een mogelijk planningsconflict detecteert met een handmatig ingeplande taak.
project.DisplayOptions.ShowTaskScheduleSuggestions = true;

// stel een waarde in die aangeeft of hyperlinks onderstreept moeten worden.
project.DisplayOptions.UnderlineHyperlinks = true;

project.Save(OutDir + "WorkWithProjectDisplayOptions.mpp", SaveFileFormat.Mpp);
```

### Zie ook

* class [ProjectDisplayOptions](../)
* namespace [Aspose.Tasks](../../projectdisplayoptions/)
* assembly [Aspose.Tasks](../../../)


