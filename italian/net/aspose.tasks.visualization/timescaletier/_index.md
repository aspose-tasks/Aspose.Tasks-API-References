---
title: "Classe TimescaleTier"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Visualization.TimescaleTier. Rappresenta un singolo livello della scala temporale in un diagramma di Gantt"
type: docs
weight: 3450
url: /it/net/aspose.tasks.visualization/timescaletier/
---
## TimescaleTier class

Rappresenta un singolo livello della scala temporale in un diagramma di Gantt.

```csharp
public sealed class TimescaleTier
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [TimescaleTier](timescaletier/#constructor)() | Inizializza una nuova istanza della classe `TimescaleTier`. |
| [TimescaleTier](timescaletier/#constructor_1)(TimescaleUnit, int) | Inizializza una nuova istanza della classe `TimescaleTier`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Alignment](../../aspose.tasks.visualization/timescaletier/alignment/) { get; set; } | Ottiene o imposta come allineare le etichette all'interno di ogni periodo di tempo del livello ([`HorizontalStringAlignment`](../horizontalstringalignment/)). |
| [Count](../../aspose.tasks.visualization/timescaletier/count/) { get; set; } | Ottiene o imposta l'intervallo dell'unità di tempo in cui mostrare le etichette per il livello. Il valore predefinito è 1. |
| [DateTimeConverter](../../aspose.tasks.visualization/timescaletier/datetimeconverter/) { get; set; } | Ottiene o imposta una funzione di callback per gestire il rendering del segno di data in questo livello. |
| [Label](../../aspose.tasks.visualization/timescaletier/label/) { get; set; } | Ottiene o imposta l'etichetta data [`DateLabel`](../datelabel/) per il livello della scala temporale. |
| [RenderLabelOnEachPage](../../aspose.tasks.visualization/timescaletier/renderlabeloneachpage/) { get; set; } | Ottiene o imposta il flag che definisce se le etichette data devono essere renderizzate su ogni pagina quando un periodo di tempo si estende su più pagine. Se il valore è 'true', quando il periodo di tempo si estende su più pagine, le etichette data per il periodo sono renderizzate su ogni pagina. Se il valore è 'false', l'etichetta data è renderizzata una sola volta in base al valore della proprietà [`Alignment`](./alignment/) property. |
| [ShowTicks](../../aspose.tasks.visualization/timescaletier/showticks/) { get; set; } | Ottiene o imposta un valore che indica se mostrare i segni di spunta che separano i periodi di tempo nel livello. |
| [Unit](../../aspose.tasks.visualization/timescaletier/unit/) { get; set; } | Ottiene o imposta l'unità della scala temporale [`TimescaleUnit`](../timescaleunit/) per il livello della scala temporale. Il valore predefinito è [`Days`](../timescaleunit/). |
| [UsesFiscalYear](../../aspose.tasks.visualization/timescaletier/usesfiscalyear/) { get; set; } | Ottiene o imposta un valore che indica se basare le etichette del livello sull'anno fiscale. |

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


