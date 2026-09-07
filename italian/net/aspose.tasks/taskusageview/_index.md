---
title: "Classe TaskUsageView"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.TaskUsageView. Rappresenta la visualizzazione dell'utilizzo delle attività in un progetto"
type: docs
weight: 2480
url: /it/net/aspose.tasks/taskusageview/
---
## TaskUsageView class

Rappresenta la vista di utilizzo dell'attività in un progetto.

```csharp
public class TaskUsageView : UsageView
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AlignDetailsData](../../aspose.tasks/usageview/aligndetailsdata/) { get; set; } | Ottiene o imposta l'allineamento dei dati dei dettagli. |
| [BottomTimescaleTier](../../aspose.tasks/usageview/bottomtimescaletier/) { get; set; } | Ottiene o imposta le impostazioni del livello inferiore della scala temporale della vista. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/) |
| [DisplayDetailsHeaderColumn](../../aspose.tasks/usageview/displaydetailsheadercolumn/) { get; set; } | Ottiene o imposta un valore che indica se visualizzare o meno la colonna intestazione dei dettagli nella vista. |
| [DisplayShortDetailHeaderNames](../../aspose.tasks/usageview/displayshortdetailheadernames/) { get; set; } | Ottiene o imposta un valore che indica se visualizzare o meno i nomi brevi dell'intestazione dei dettagli. |
| [FieldCollection](../../aspose.tasks/taskusageview/fieldcollection/) { get; } | Ottiene l'oggetto [`TaskUsageViewFieldCollection`](../taskusageviewfieldcollection/) di questo TaskUsageView. |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | Ottiene o imposta un filtro utilizzato in una singola vista. |
| [Group](../../aspose.tasks/view/group/) { get; set; } | Ottiene o imposta un gruppo della singola vista. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | Ottiene o imposta un valore che indica se Microsoft Project evidenzia il filtro per una singola vista. |
| [MiddleTimescaleTier](../../aspose.tasks/usageview/middletimescaletier/) { get; set; } | Ottiene o imposta le impostazioni del livello intermedio della scala temporale della vista. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/). |
| [Name](../../aspose.tasks/view/name/) { get; set; } | Ottiene o imposta il nome di un oggetto View. |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | Ottiene un'istanza della classe [`PageInfo`](../view/pageinfo/). Rappresenta i dati di configurazione della pagina presenti nel formato file mpp. |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | Ottiene il genitore dell'oggetto View. Solo lettura [`Project`](../project/). |
| [RepeatDetailsHeaderOnAllRows](../../aspose.tasks/usageview/repeatdetailsheaderonallrows/) { get; set; } | Ottiene o imposta un valore che indica se ripetere l'intestazione dei dettagli su tutte le righe di assegnazione o meno. |
| [Screen](../../aspose.tasks/view/screen/) { get; } | Ottiene il tipo di schermo per la singola vista. Solo lettura [`ViewScreen`](../viewscreen/). |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | Ottiene o imposta un valore che indica se Microsoft Project mostra il nome della singola vista nelle liste a discesa Vista o Altre viste nel Ribbon. |
| [Table](../../aspose.tasks/view/table/) { get; set; } | Ottiene o imposta una tabella della singola vista. |
| [TimescaleSizePercentage](../../aspose.tasks/usageview/timescalesizepercentage/) { get; set; } |  |
| [TopTimescaleTier](../../aspose.tasks/usageview/toptimescaletier/) { get; set; } | Ottiene o imposta le impostazioni del livello superiore della scala temporale della vista. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/). |
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

Mostra come renderizzare la visualizzazione dell'utilizzo delle attività con le impostazioni della scala temporale definite nelle impostazioni della vista.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = project.Views.ToList()[2] as TaskUsageView;

view.TopTimescaleTier.Unit = TimescaleUnit.None;

view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
view.MiddleTimescaleTier.Label = DateLabel.WeekDddMDd;
view.MiddleTimescaleTier.Count = 1;

view.BottomTimescaleTier.Unit = TimescaleUnit.Days;
view.BottomTimescaleTier.Label = DateLabel.DayMmDd;
view.BottomTimescaleTier.Count = 1;

// Definisci le SaveOptions e specifica che le impostazioni della scala temporale TaskUsageView devono essere utilizzate.
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    PresentationFormat = PresentationFormat.TaskUsage
};

project.Save(OutDir + "TaskUsageView_CustomTimescale_out.pdf", options);
```

Mostra come renderizzare la vista TaskUsageView con impostazioni della scala temporale predefinite.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

// Definisci le SaveOptions e specifica le impostazioni predefinite del TimeScale 'Days'.
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Days,

    // Imposta il formato Presentation su TaskUsage
    PresentationFormat = PresentationFormat.TaskUsage
};

var outputProject = "TaskUsageView_result_days_out.pdf";
project.Save(OutDir + outputProject, options);

// Imposta le impostazioni della Timescale su ThirdsOfMonths
options.Timescale = Timescale.ThirdsOfMonths;

outputProject = "TaskUsageView_result_thirdsOfMonths_out.pdf";
project.Save(OutDir + outputProject, options);

// Imposta le impostazioni della Timescale su Months
options.Timescale = Timescale.Months;

outputProject = "TaskUsageView_result_months_out.pdf";
project.Save(OutDir + outputProject, options);
```

### Vedi anche

* class [UsageView](../usageview/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


