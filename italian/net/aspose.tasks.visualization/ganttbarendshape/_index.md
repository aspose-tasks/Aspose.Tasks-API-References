---
title: "Enum GanttBarEndShape"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.Visualization.GanttBarEndShape enum. Rappresenta la forma finale nelle barre e nei punti di avanzamento nelle linee di avanzamento"
type: docs
weight: 3030
url: /it/net/aspose.tasks.visualization/ganttbarendshape/
---
## GanttBarEndShape enumeration

Rappresenta la forma finale nelle barre e nei punti di avanzamento nelle linee di progresso.

```csharp
public enum GanttBarEndShape
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| ArrowDown | `14` | Indica la freccia che punta verso il basso Gantt bar end shape. |
| ArrowUp | `8` | Indica la freccia che punta verso l'alto Gantt bar end shape. |
| CaretDownTop | `9` | Indica Caret che punta verso il basso nella metà superiore della barra Gantt bar end shape. |
| CaretUpBottom | `10` | Indica Caret che punta verso l'alto nella metà inferiore della barra Gantt bar end shape. |
| Circle | `19` | Indica cerchio Gantt bar end shape. |
| CircleArrowDown | `18` | Indica freccia cerchiata che punta verso il basso Gantt bar end shape. |
| CircleArrowUp | `17` | Indica freccia cerchiata che punta verso l'alto Gantt bar end shape. |
| CircleDiamond | `13` | Indica diamante cerchiato Gantt bar end shape. |
| CircleTriangleDown | `16` | Indica triangolo cerchiato che punta verso il basso Gantt bar end shape. |
| CircleTriangleUp | `15` | Indica triangolo cerchiato che punta verso l'alto Gantt bar end shape. |
| Diamond | `3` | Indica diamante Gantt bar end shape. |
| HouseDown | `2` | Indica casa capovolta Gantt bar end shape. |
| HouseUp | `1` | Indica casa Gantt bar end shape. |
| LeftBracket | `21` | Indica parentesi sinistra Gantt bar end shape. |
| LeftFade | `23` | Indica sfumatura sinistra Gantt bar end shape. |
| LineShape | `11` | Indica linea Gantt bar end shape. |
| NoBarEndShape | `0` | Indica nessuna Gantt bar end shape. |
| RightBracket | `22` | Indica parentesi destra Gantt bar end shape. |
| RightFade | `24` | Indica sfumatura destra Gantt bar end shape. |
| Square | `12` | Indica quadrato Gantt bar end shape. |
| Star | `20` | Indica stella Gantt bar end shape. |
| TriangleDown | `5` | Indica triangolo che punta verso il basso Gantt bar end shape. |
| TriangleLeft | `7` | Indica la forma a triangolo che punta a sinistra alla fine della barra Gantt. |
| TriangleRight | `6` | Indica la forma a triangolo che punta a destra alla fine della barra Gantt. |
| TriangleUp | `4` | Indica triangolo cerchiato che punta verso l'alto Gantt bar end shape. |

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


