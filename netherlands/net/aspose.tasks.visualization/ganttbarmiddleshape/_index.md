---
title: "Enum GanttBarMiddleShape"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Visualization.GanttBarMiddleShape enum. Specificeert de middelste vorm van een balk"
type: docs
weight: 3050
url: /nl/net/aspose.tasks.visualization/ganttbarmiddleshape/
---
## GanttBarMiddleShape enumeration

Specificeert de middelste vorm van een balk.

```csharp
public enum GanttBarMiddleShape
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| LineBottom | `7` | Geeft onder uitgelijnde lijngvorm aan. |
| LineMiddle | `6` | Geeft centraal uitgelijnde lijngvorm aan. |
| LineTop | `5` | Geeft boven uitgelijnde lijngvorm aan. |
| None | `0` | Geeft lege vorm aan. |
| RectangleBar | `1` | Geeft volledige hoogte rechthoekige balkvorm aan. |
| RectangleBottom | `4` | Geeft onderaan uitgelijnde halve hoogte rechthoekige balkvorm aan. |
| RectangleMiddle | `3` | Geeft gecentreerde 1/3 hoogte rechthoekige balkvorm aan. |
| RectangleTop | `2` | Geeft boven uitgelijnde halve hoogte rechthoekige balkvorm aan. |

## Voorbeelden

Toont hoe aangepaste balkstijlen van de Gantt-diagram projectweergave in te stellen.

```csharp
public void ImplementCustomBarStyle()
{
    try
    {
        var project = new Project(DataDir + "Blank2010.mpp");
        project.RootTask.Children.Add("Task");

        var view = (GanttChartView)project.DefaultView;
        var custom = GetCustomBarStyle();

        // Voeg de aangepaste balkstijl toe aan de collectie van aangepaste balken van de projectweergave.
        view.CustomBarStyles.Add(custom);

        SimpleSaveOptions options = new MPPSaveOptions
        {
            WriteViewData = true
        };

        project.Save(OutDir + "ImplementCustomBarStyleWriting_out.mpp", options);
    }
    catch (NotSupportedException ex)
    {
        Console.WriteLine(
            ex.Message
            + "\nThis example will only work if you apply a valid Aspose License. You can purchase full license or get 30 day temporary license from http://www.aspose.com/purchase/default.aspx.");
    }
}

public static GanttBarStyle GetCustomBarStyle()
{
    var style = new GanttBarStyle
    {
        ShowForTaskUid = 1,
        MiddleShape = GanttBarMiddleShape.RectangleBottom,
        MiddleFillPattern = GanttBarFillPattern.MediumFill,
        MiddleShapeColor = Color.Blue,

        StartShape = GanttBarEndShape.ArrowDown,
        StartShapeColor = Color.Red,

        EndShape = GanttBarEndShape.ArrowUp,
        EndShapeColor = Color.Yellow,

        LeftField = Field.TaskResourceNames,
        RightField = Field.TaskName,
        TopField = Field.TaskStart,
        BottomField = Field.TaskFinish,
        InsideField = Field.TaskDuration
    };

    return style;
}
```

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


