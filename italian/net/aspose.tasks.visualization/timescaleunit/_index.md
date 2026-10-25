---
title: "Enum TimescaleUnit"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.Visualization.TimescaleUnit enum. Specifica l'unità di tempo per qualsiasi livello di una scala temporale in un diagramma di Gantt o in un'altra vista a fasi temporali."
type: docs
weight: 3460
url: /it/net/aspose.tasks.visualization/timescaleunit/
---
## TimescaleUnit enumeration

Specifica l'unità di tempo per qualsiasi livello di una scala temporale in un diagramma di Gantt o in un'altra visualizzazione a fasi temporali.

```csharp
public enum TimescaleUnit
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `-1` | Indica Nessuno. Il livello della scala temporale è nascosto. |
| Minutes | `0` | Indica l'unità di tempo Minuti. |
| Hours | `1` | Indica l'unità di tempo Ore. |
| Days | `2` | Indica l'unità di tempo Giorni. |
| Weeks | `3` | Indica l'unità di tempo Settimane. |
| ThirdsOfMonths | `4` | Indica l'unità di tempo Terzi di mese. |
| Months | `5` | Indica l'unità di tempo Mesi. |
| Quarters | `6` | Indica l'unità di tempo Trimestri di anno. |
| HalfYears | `7` | Indica l'unità di tempo Semestri. |
| Years | `8` | Indica l'unità di tempo Anni. |

## Esempi

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


