---
title: "GanttChartView.TopTimescaleTier"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà GanttChartView. Ottiene o imposta le impostazioni del livello superiore della scala temporale della vista. TimescaleTier"
type: docs
weight: 190
url: /it/net/aspose.tasks/ganttchartview/toptimescaletier/
---
## GanttChartView.TopTimescaleTier property

Ottiene o imposta le impostazioni del tier di scala temporale superiore della visualizzazione. [`TimescaleTier`](../../../aspose.tasks.visualization/timescaletier/).

```csharp
public TimescaleTier TopTimescaleTier { get; set; }
```

## Esempi

Mostra come modificare i livelli della scala temporale.

```csharp
var project = new Project();

// Inizializza la vista Gantt Chart
var view = new GanttChartView
{
    TopTimescaleTier = new TimescaleTier(),
    MiddleTimescaleTier = new TimescaleTier(),
    BottomTimescaleTier = new TimescaleTier()
};

// imposta il conteggio della scala temporale
view.TopTimescaleTier.Count = 2;
view.TopTimescaleTier.Unit = TimescaleUnit.Quarters;
view.TopTimescaleTier.Label = DateLabel.QuarterQQyy;
view.TopTimescaleTier.ShowTicks = false;

view.MiddleTimescaleTier.Count = 2;
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
view.MiddleTimescaleTier.ShowTicks = false;

view.BottomTimescaleTier.Unit = TimescaleUnit.Days;
view.BottomTimescaleTier.Label = DateLabel.DayDdd;
view.BottomTimescaleTier.Count = 2;
view.BottomTimescaleTier.ShowTicks = false;

// aggiungi la vista Gantt Chart al progetto
project.Views.Add(view);

// aggiungi alcuni dati di test al progetto
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");
task1.Set(Tsk.Duration, task1.ParentProject.GetDuration(24, TimeUnitType.Hour));
task2.Set(Tsk.Duration, task1.ParentProject.GetDuration(40, TimeUnitType.Hour));

// Usa l'opzione 'Timescale.DefinedInView' per renderizzare le scale temporali utilizzando le impostazioni della scala temporale che abbiamo impostato (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier).
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    StartDate = DateTime.Now.AddDays(-30),
    EndDate = DateTime.Now.AddDays(30)
};

project.Save(OutDir + "WorkWithTimescaleTier_out.pdf", pdfSaveOptions);
```

Mostra come personalizzare le etichette del livello della scala temporale.

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");

// Aggiungi collegamenti alle attività
project.TaskLinks.Add(project.RootTask.Children.Add("Task 1"), project.RootTask.Children.Add("Task 2"));

var view = (GanttChartView)project.DefaultView;

// regola i livelli della scala temporale

// regola il livello superiore
// imposta il livello superiore della scala temporale della vista del diagramma di Gantt.
view.MiddleTimescaleTier = new TimescaleTier();
// imposta l'unità della scala temporale <see cref=\"T:Aspose.Tasks.Visualization.TimescaleUnit\" /> per il livello della scala temporale.
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
// imposta l'intervallo dell'unità di tempo in cui mostrare le etichette per il livello.
view.MiddleTimescaleTier.Count = 1;
// imposta l'etichetta data <see cref=\"T:Aspose.Tasks.Visualization.DateLabel\" /> per il livello della scala temporale.
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
// imposta come allineare le etichette all'interno di ogni periodo di tempo del livello (<see cref=\"T:System.Drawing.StringAlignment\" />).
view.MiddleTimescaleTier.Alignment = HorizontalStringAlignment.Center;
// imposta un valore che indica se mostrare i segni di spunta che separano i periodi di tempo nel livello.
view.MiddleTimescaleTier.ShowTicks = true;
// imposta un valore che indica se basare le etichette del livello sull'anno fiscale.
view.MiddleTimescaleTier.UsesFiscalYear = true;

// aggiunto per una migliore visualizzazione
view.TopTimescaleTier = new TimescaleTier(TimescaleUnit.Months, 1);

// personalizza le date del livello intermedio
view.TopTimescaleTier.DateTimeConverter = date =>
    new[] { "Янв.", "Фев.", "Мар.", "Апр.", "Май", "Июнь", "Июль", "Авг.", "Сен.", "Окт.", "Ноя.", "Дек." }[date.Month - 1];

project.Set(Prj.TimescaleStart, new DateTime(2012, 7, 30));
project.Set(Prj.TimescaleFinish, new DateTime(2012, 10, 6));

// Usa l'opzione 'Timescale.DefinedInView' per renderizzare le scale temporali utilizzando le impostazioni della scala temporale definite nella vista (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier).
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "CustomizeTimescaleTierLabels_out.pdf", pdfSaveOptions);
```

### Vedi anche

* class [TimescaleTier](../../../aspose.tasks.visualization/timescaletier/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


