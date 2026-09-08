---
title: "Klasse ProjectDisplayOptions"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.ProjectDisplayOptions‑klasse. Vertegenwoordigt de weergave‑opties voor een project‑instantie"
type: docs
weight: 1450
url: /nl/net/aspose.tasks/projectdisplayoptions/
---
## ProjectDisplayOptions class

Stelt de weergave‑opties voor een project‑instantie voor.

```csharp
public class ProjectDisplayOptions
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [ProjectDisplayOptions](projectdisplayoptions/)() | Initialiseert een nieuw exemplaar van de `ProjectDisplayOptions`‑klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [AddSpaceBeforeLabel](../../aspose.tasks/projectdisplayoptions/addspacebeforelabel/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of er een spatie vóór de numerieke waarde en de tijdsaanduiding moet worden geplaatst (1 wk in plaats van 1wk). |
| [DayLabel](../../aspose.tasks/projectdisplayoptions/daylabel/) { get; set; } | Haalt op of stelt in hoe het daglabel wordt weergegeven. |
| [HourLabel](../../aspose.tasks/projectdisplayoptions/hourlabel/) { get; set; } | Haalt op of stelt in hoe het uurlabel wordt weergegeven. |
| [MinuteLabel](../../aspose.tasks/projectdisplayoptions/minutelabel/) { get; set; } | Haalt op of stelt in hoe het minutenlabel wordt weergegeven. |
| [MonthLabel](../../aspose.tasks/projectdisplayoptions/monthlabel/) { get; set; } | Haalt op of stelt in hoe het maandlabel wordt weergegeven. |
| [ShowProjectSummaryTask](../../aspose.tasks/projectdisplayoptions/showprojectsummarytask/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of samenvattende informatie over een heel project op één rij moet worden weergegeven met een eigen samenvattende taakbalk bovenaan de Gantt‑diagramweergave. |
| [ShowTaskScheduleSuggestions](../../aspose.tasks/projectdisplayoptions/showtaskschedulesuggestions/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of suggesties moeten worden getoond wanneer Project een mogelijk planningsconflict identificeert met een handmatig geplande taak. Deze optie is beschikbaar voor Project 2010 en latere versies. |
| [ShowTaskScheduleWarnings](../../aspose.tasks/projectdisplayoptions/showtaskschedulewarnings/) { get; set; } | Haalt een waarde op of stelt deze in die aangeeft of waarschuwingen moeten worden weergegeven wanneer Project een mogelijk planningsconflict detecteert met een handmatig ingeplande taak. Deze optie is beschikbaar voor Project 2010 en later. |
| [UnderlineHyperlinks](../../aspose.tasks/projectdisplayoptions/underlinehyperlinks/) { get; set; } | Haalt een waarde op of stelt deze in die aangeeft of hyperlinks onderstreept moeten worden. |
| [WeekLabel](../../aspose.tasks/projectdisplayoptions/weeklabel/) { get; set; } | Haalt op of stelt in hoe het weeklabel wordt weergegeven. |
| [YearLabel](../../aspose.tasks/projectdisplayoptions/yearlabel/) { get; set; } | Haalt op of stelt in hoe het jaarlabel wordt weergegeven. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


