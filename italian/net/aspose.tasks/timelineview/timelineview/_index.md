---
title: "TimelineView.TimelineView"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Costruttore TimelineView. Inizializza una nuova istanza della classe TimelineView"
type: docs
weight: 10
url: /it/net/aspose.tasks/timelineview/timelineview/
---
## TimelineView constructor

Inizializza una nuova istanza della classe [`TimelineView`](../).

```csharp
public TimelineView()
```

## Esempi

Mostra come lavorare con &lt;see cref="Aspose.Tasks.TimelineView" /&gt;.

```csharp
var project = new Project();

// inizializza una vista timeline
var view = new TimelineView();

// imposta un valore che indica come formattare le date nella vista Timeline.
view.DateFormat = DateFormat.DateDddDd;
// imposta un valore che indica se visualizzare attività sovrapposte su più righe.
view.DisplayOverlapped = true;
// imposta un valore che indica se mostrare il controllo pan e zoom.
view.ShowPanZoom = true;
// imposta un valore che indica se mostrare la scala temporale.
view.ShowTimescale = true;
// imposta un valore che indica se visualizzare una linea che rappresenta oggi.
view.ShowToday = true;
// imposta un valore che indica quante linee sono usate per visualizzare le attività in una timeline.
view.TextLinesCount = 2;

// ottiene un valore che indica se visualizzare attività sovrapposte su più righe.
Console.WriteLine("Show Dates: " + view.ShowDates);

// aggiungi la vista al progetto
project.Views.Add(view);

// aggiungi alcuni dati di test al progetto
var task1 = project.RootTask.Children.Add("Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 4, 29, 8, 0, 0));
task1.Set(Tsk.Duration, task1.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Start, new DateTime(2020, 4, 29, 8, 0, 0));
task2.Set(Tsk.Duration, task1.ParentProject.GetDuration(40, TimeUnitType.Hour));

project.Save(OutDir + "SetTimeScaleCount_out.pdf", SaveFileFormat.Pdf);
```

### Vedi anche

* class [TimelineView](../)
* namespace [Aspose.Tasks](../../timelineview/)
* assembly [Aspose.Tasks](../../../)


