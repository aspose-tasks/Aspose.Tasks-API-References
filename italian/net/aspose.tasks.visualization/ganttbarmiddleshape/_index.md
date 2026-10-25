---
title: "Enum GanttBarMiddleShape"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.Visualization.GanttBarMiddleShape enum. Specifica la forma centrale di una barra"
type: docs
weight: 3050
url: /it/net/aspose.tasks.visualization/ganttbarmiddleshape/
---
## GanttBarMiddleShape enumeration

Specifica la forma centrale di una barra.

```csharp
public enum GanttBarMiddleShape
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| LineBottom | `7` | Indica la forma a linea allineata in basso. |
| LineMiddle | `6` | Indica la forma a linea allineata al centro. |
| LineTop | `5` | Indica la forma a linea allineata in alto. |
| None | `0` | Indica forma vuota. |
| RectangleBar | `1` | Indica forma a barra rettangolare a piena altezza. |
| RectangleBottom | `4` | Indica forma a barra rettangolare a mezza altezza allineata in basso. |
| RectangleMiddle | `3` | Indica forma a barra rettangolare a 1/3 di altezza allineata al centro. |
| RectangleTop | `2` | Indica la forma a rettangolo di metà altezza allineata in alto. |

## Esempi

Mostra come impostare gli stili di barra personalizzati della vista progetto del diagramma di Gantt.

```csharp
public void ImplementCustomBarStyle()
{
    try
    {
        var project = new Project(DataDir + "Blank2010.mpp");
        project.RootTask.Children.Add("Task");

        var view = (GanttChartView)project.DefaultView;
        var custom = GetCustomBarStyle();

        // Aggiungi lo stile di barra personalizzato alla collezione di barre personalizzate della vista progetto
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

Mostra come utilizzare gli stili di barra personalizzati della vista del diagramma di Gantt.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var ganttChartView = (GanttChartView)project.Views.First(v => v.Name == "Gantt &Chart");
PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.ViewSettings = ganttChartView;

// Gli stili di barra possono essere specifici per attività (situati in GanttChartView.CustomBarStyles)
// o specifici per categoria (situati in GanttChartView.BarStyles)
foreach (GanttBarStyle ganttBarStyle in ganttChartView.CustomBarStyles)
{
    if (ganttBarStyle.ShowForTaskUid != 4)
    {
        continue;
    }

    // Per scopi dimostrativi stiamo modificando lo stile per l'attività con ID univoco = 4
    // Qui impostiamo il campo (TaskName) per renderlo a sinistra della barra dell'attività.
    ganttBarStyle.LeftField = Field.TaskName;
    // Qui impostiamo un convertitore personalizzato per controllare quale testo deve essere visualizzato all'interno della barra dell'attività.
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

    // Per scopi dimostrativi stiamo modificando gli stili applicabili alle attività milestone.

    ganttBarStyle.StartShape = GanttBarEndShape.Diamond;
    ganttBarStyle.RightField = Field.TaskActualFinish;
    ganttBarStyle.TopBarTextConverter = task => task.Get(Tsk.ActualStart).Day.ToString();
}

project.Save(OutDir + "WorkWithGanttChartViewBarStyles_out.pdf", saveOptions);
```

### Vedi anche

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


