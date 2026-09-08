---
title: "Enum GanttBarEndShape"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Visualization.GanttBarEndShape enum. Vertegenwoordigt eindvorm in balken en voortgangspunten in voortgangslijnen"
type: docs
weight: 3030
url: /nl/net/aspose.tasks.visualization/ganttbarendshape/
---
## GanttBarEndShape enumeration

Stelt de eindvorm in balken en voortgangspunten in voortgangslijnen voor.

```csharp
public enum GanttBarEndShape
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| ArrowDown | `14` | Geeft de pijl naar beneden Gantt-balk eindvorm aan. |
| ArrowUp | `8` | Geeft de pijl naar boven Gantt-balk eindvorm aan. |
| CaretDownTop | `9` | Geeft caret naar beneden op de bovenste helft van de balk Gantt-balk eindvorm aan. |
| CaretUpBottom | `10` | Geeft caret naar boven op de onderste helft van de balk Gantt-balk eindvorm aan. |
| Circle | `19` | Geeft cirkel Gantt-balk eindvorm aan. |
| CircleArrowDown | `18` | Geeft omcirkelde pijl naar beneden Gantt-balk eindvorm aan. |
| CircleArrowUp | `17` | Geeft omcirkelde pijl naar boven Gantt-balk eindvorm aan. |
| CircleDiamond | `13` | Geeft omcirkelde diamant Gantt-balk eindvorm aan. |
| CircleTriangleDown | `16` | Geeft omcirkelde driehoek naar beneden Gantt-balk eindvorm aan. |
| CircleTriangleUp | `15` | Geeft omcirkelde driehoek naar boven Gantt-balk eindvorm aan. |
| Diamond | `3` | Geeft diamant Gantt-balk eindvorm aan. |
| HouseDown | `2` | Geeft ondersteboven huis Gantt-balk eindvorm aan. |
| HouseUp | `1` | Geeft huis Gantt-balk eindvorm aan. |
| LeftBracket | `21` | Geeft linker haakje Gantt-balk eindvorm aan. |
| LeftFade | `23` | Geeft linker vervaging Gantt-balk eindvorm aan. |
| LineShape | `11` | Geeft lijn Gantt-balk eindvorm aan. |
| NoBarEndShape | `0` | Geeft geen Gantt-balk eindvorm aan. |
| RightBracket | `22` | Geeft rechter haakje Gantt-balk eindvorm aan. |
| RightFade | `24` | Geeft rechter vervaging Gantt-balk eindvorm aan. |
| Square | `12` | Geeft vierkant Gantt-balk eindvorm aan. |
| Star | `20` | Geeft ster Gantt-balk eindvorm aan. |
| TriangleDown | `5` | Geeft driehoek naar beneden Gantt-balk eindvorm aan. |
| TriangleLeft | `7` | Geeft de naar links wijzende driehoek aan als eindvorm van de Gantt-balk. |
| TriangleRight | `6` | Geeft de naar rechts wijzende driehoek aan als eindvorm van de Gantt-balk. |
| TriangleUp | `4` | Geeft omcirkelde driehoek naar boven Gantt-balk eindvorm aan. |

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


