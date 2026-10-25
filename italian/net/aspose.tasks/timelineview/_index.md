---
title: "Classe TimelineView"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.TimelineView. Rappresenta una vista della timeline di un progetto"
type: docs
weight: 2580
url: /it/net/aspose.tasks/timelineview/
---
## TimelineView class

Rappresenta una vista della timeline di un progetto.

```csharp
public class TimelineView : View
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [TimelineView](timelineview/)() | Inizializza una nuova istanza della classe `TimelineView`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DateFormat](../../aspose.tasks/timelineview/dateformat/) { get; set; } | Ottiene o imposta un valore che indica come formattare le date nella vista Timeline. |
| [DisplayOverlapped](../../aspose.tasks/timelineview/displayoverlapped/) { get; set; } | Ottiene o imposta un valore che indica se visualizzare attività sovrapposte su più righe. |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | Ottiene o imposta un filtro utilizzato in una singola vista. |
| [Group](../../aspose.tasks/view/group/) { get; set; } | Ottiene o imposta un gruppo della singola vista. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | Ottiene o imposta un valore che indica se Microsoft Project evidenzia il filtro per una singola vista. |
| [Name](../../aspose.tasks/view/name/) { get; set; } | Ottiene o imposta il nome di un oggetto View. |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | Ottiene un'istanza della classe [`PageInfo`](../view/pageinfo/). Rappresenta i dati di configurazione della pagina presenti nel formato file mpp. |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | Ottiene il genitore dell'oggetto View. Solo lettura [`Project`](../project/). |
| [Screen](../../aspose.tasks/view/screen/) { get; } | Ottiene il tipo di schermo per la singola vista. Solo lettura [`ViewScreen`](../viewscreen/). |
| [ShowDates](../../aspose.tasks/timelineview/showdates/) { get; } | Ottiene un valore che indica se mostrare le date. |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | Ottiene o imposta un valore che indica se Microsoft Project mostra il nome della singola vista nelle liste a discesa Vista o Altre viste nel Ribbon. |
| [ShowPanZoom](../../aspose.tasks/timelineview/showpanzoom/) { get; set; } | Ottiene o imposta un valore che indica se mostrare il controllo pan e zoom. |
| [ShowTimescale](../../aspose.tasks/timelineview/showtimescale/) { get; set; } | Ottiene o imposta un valore che indica se mostrare la scala temporale. |
| [ShowToday](../../aspose.tasks/timelineview/showtoday/) { get; set; } | Ottiene o imposta un valore che indica se visualizzare una linea che rappresenta oggi. |
| [Table](../../aspose.tasks/view/table/) { get; set; } | Ottiene o imposta una tabella della singola vista. |
| [TextLinesCount](../../aspose.tasks/timelineview/textlinescount/) { get; set; } | Ottiene o imposta un valore che indica quante linee sono usate per visualizzare le attività in una timeline. |
| [Type](../../aspose.tasks/view/type/) { get; } | Ottiene il tipo di elemento nella singola vista, come attività o risorse. Solo lettura [`ItemType`](../itemtype/). |
| [Uid](../../aspose.tasks/view/uid/) { get; } | Ottiene l'identificatore univoco di una vista. |
| [VisualObjectsPlacements](../../aspose.tasks/view/visualobjectsplacements/) { get; } | Ottiene una raccolta di oggetti che rappresentano la posizione e l'aspetto di [`OleObject`](../oleobject/) nella vista. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [CompareTo](../../aspose.tasks/view/compareto/)(View) | Confronta l'istanza corrente con un altro oggetto dello stesso tipo e restituisce un intero che indica se l'istanza corrente precede, segue o si trova nella stessa posizione nell'ordine di ordinamento rispetto all'altro oggetto. |
| override [Equals](../../aspose.tasks/view/equals/)(object) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| override [GetHashCode](../../aspose.tasks/view/gethashcode/)() | Restituisce un valore di codice hash per l'istanza della classe [`Resource`](../resource/). |

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

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


