---
title: "GanttBarStyle.BottomBarTextConverter"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "GanttBarStyle eigenschap. Haalt op of stelt een door de gebruiker gedefinieerde converter in om tekst te verkrijgen die onder de taakbalk wordt weergegeven. Overschrijft de waarde van de BottomField eigenschap."
type: docs
weight: 20
url: /nl/net/aspose.tasks.visualization/ganttbarstyle/bottombartextconverter/
---
## GanttBarStyle.BottomBarTextConverter property

Haalt op of stelt een door de gebruiker gedefinieerde converter in om tekst te verkrijgen die onder de balk van de taak wordt weergegeven. Overschrijft de waarde van [`BottomField`](../bottomfield/) eigenschap.

```csharp
public TaskBarTextConverter BottomBarTextConverter { get; set; }
```

## Opmerkingen

Wordt niet opgeslagen in MPP-indeling.

## Voorbeelden

Toont hoe aangepaste balkstijlen van de Gantt-diagramweergave te gebruiken.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var ganttChartView = (GanttChartView)project.Views.First(v => v.Name == "Gantt &Chart");
PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.ViewSettings = ganttChartView;

// Balkstijlen kunnen taak‑specifiek zijn (te vinden in GanttChartView.CustomBarStyles).
// of categorie‑specifiek (te vinden in GanttChartView.BarStyles).
foreach (GanttBarStyle ganttBarStyle in ganttChartView.CustomBarStyles)
{
    if (ganttBarStyle.ShowForTaskUid != 4)
    {
        continue;
    }

    // Voor demonstratiedoeleinden passen we de stijl aan voor taak met unieke ID = 4.
    // Hier stellen we het veld (TaskName) in om links van de taakbalk te worden weergegeven.
    ganttBarStyle.LeftField = Field.TaskName;
    // Hier stellen we een aangepaste converter in om te bepalen welke tekst binnen de taakbalk moet worden weergegeven.
    ganttBarStyle.InsideBarTextConverter = task => "Hours rem.: " + (int)task.Get(Tsk.RemainingWork).TimeSpan.TotalHours;

    ganttBarStyle.MiddleShapeColor = Color.Green;
    ganttBarStyle.MiddleShape = GanttBarMiddleShape.LineTop;
    ganttBarStyle.StartShape = GanttBarEndShape.LeftBracket;
    ganttBarStyle.StartShapeColor = Color.Aqua;
    ganttBarStyle.EndShape = GanttBarEndShape.RightBracket;
    ganttBarStyle.EndShapeColor = Color.Aquamarine;
}

foreach (GanttBarStyle ganttBarStyle in ganttChartView.BarStyles)
{
    if (!ganttBarStyle.ShowForCategories.Contains(GanttBarShowFor.Milestone))
    {
        continue;
    }

    // Voor demonstratiedoeleinden passen we stijlen aan die van toepassing zijn op mijlpaaltaak.

    ganttBarStyle.StartShape = GanttBarEndShape.Diamond;
    ganttBarStyle.RightField = Field.TaskActualFinish;
    ganttBarStyle.TopBarTextConverter = task => task.Get(Tsk.ActualStart).Day.ToString();
}

project.Save(OutDir + "WorkWithGanttChartViewBarStyles_out.pdf", saveOptions);
```

### Zie ook

* delegate [TaskBarTextConverter](../../taskbartextconverter/)
* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


