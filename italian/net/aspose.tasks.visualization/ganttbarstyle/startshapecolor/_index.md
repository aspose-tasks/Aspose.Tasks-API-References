---
title: "GanttBarStyle.StartShapeColor"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà GanttBarStyle. Ottiene o imposta un colore della forma iniziale"
type: docs
weight: 230
url: /it/net/aspose.tasks.visualization/ganttbarstyle/startshapecolor/
---
## GanttBarStyle.StartShapeColor property

Ottiene o imposta il colore della forma di inizio.

```csharp
public Color StartShapeColor { get; set; }
```

## Esempi

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

Mostra come leggere gli stili della barra personalizzati di una vista.

```csharp
var project = new Project(DataDir + "CustomBarStyle.mpp");

var view = (GanttChartView)project.DefaultView;
Console.WriteLine("Custom bar styles count: {0}", view.CustomBarStyles.Count);

var style1 = view.CustomBarStyles[0];
Console.WriteLine("Style1.ParentStyle Name: {0}", style1.ParentStyle.Name);
Console.WriteLine("Style1.LeftField: {0}", style1.LeftField);
Console.WriteLine("Style1.RightField: {0}", style1.RightField);
Console.WriteLine("Style1.TopField: {0}", style1.TopField);
Console.WriteLine("Style1.BottomField: {0}", style1.BottomField);
Console.WriteLine("Style1.InsideField: {0}", style1.InsideField);
Console.WriteLine("Style1.From: {0}", style1.From);
Console.WriteLine("Style1.To: {0}", style1.To);
Console.WriteLine("Style1.Row: {0}", style1.Row);

var style2 = view.CustomBarStyles[1];
Console.WriteLine("Style2.LeftField: {0}", style2.LeftField);
Console.WriteLine("Style2.RightField: {0}", style2.RightField);
Console.WriteLine("Style2.TopField: {0}", style2.TopField);
Console.WriteLine("Style2.BottomField: {0}", style2.BottomField);
Console.WriteLine("Style2.InsideField: {0}", style2.InsideField);
Console.WriteLine("Style2.From: {0}", style2.From);
Console.WriteLine("Style2.To: {0}", style2.To);
Console.WriteLine("Style2.Row: {0}", style1.Row);

var style3 = view.CustomBarStyles[2];
Console.WriteLine("Style3.LeftField: {0}", style3.LeftField);
Console.WriteLine("Style3.RightField: {0}", style3.RightField);
Console.WriteLine("Style3.TopField: {0}", style3.TopField);
Console.WriteLine("Style3.BottomField: {0}", style3.BottomField);
Console.WriteLine("Style3.InsideField: {0}", style3.InsideField);

Console.WriteLine("Style3.StartShape: {0}", style3.StartShape);
Console.WriteLine("Style3.StartShapeType: {0}", style3.StartShapeType);
Console.WriteLine("Style3.StartShapeColor: {0}", style3.StartShapeColor);

Console.WriteLine("Style3.EndShape: {0}", style3.EndShape);
Console.WriteLine("Style3.EndShapeType: {0}", style3.EndShapeType);
Console.WriteLine("Style3.EndShapeColor: {0}", style3.EndShapeColor);

Console.WriteLine("Style3.MiddleShape: {0}", style3.MiddleShape);
Console.WriteLine("Style3.MiddleFillPattern: {0}", style3.MiddleFillPattern);
Console.WriteLine("Style3.MiddleShapeColor: {0}", style3.MiddleShapeColor);
Console.WriteLine("Style3.From: {0}", style3.From);
Console.WriteLine("Style3.To: {0}", style3.To);
Console.WriteLine("Style3.Row: {0}", style1.Row);
```

### Vedi anche

* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


