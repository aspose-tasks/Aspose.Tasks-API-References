---
title: Class GanttChartView
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: Aspose.Tasks.GanttChartView classe. Rappresenta una vista Diagramma di Gantt.
type: docs
weight: 700
url: /it/net/aspose.tasks/ganttchartview/
---
## GanttChartView class

Rappresenta una vista Diagramma di Gantt.

```csharp
public class GanttChartView : View
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [GanttChartView](ganttchartview/)() | Inizializza una nuova istanza di`GanttChartView` classe. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AutoFilters](../../aspose.tasks/ganttchartview/autofilters/) { get; } | Ottiene un elenco di filtri automatici di una visualizzazione Diagramma di Gantt. |
| [BarRounding](../../aspose.tasks/ganttchartview/barrounding/) { get; set; } | Ottiene o imposta un valore che indica se le barre sono arrotondate al giorno più vicino. Il valore predefinito è True. |
| [BarSize](../../aspose.tasks/ganttchartview/barsize/) { get; set; } | Ottiene o imposta l'altezza, in punti, delle barre di Gantt nel diagramma di Gantt. |
| [BarStyles](../../aspose.tasks/ganttchartview/barstyles/) { get; } | Ottiene un elenco di stili di barra principali (comuni) della visualizzazione Diagramma di Gantt. [`GanttBarStyle`](../../aspose.tasks.visualization/ganttbarstyle/) . |
| [BottomTimescaleTier](../../aspose.tasks/ganttchartview/bottomtimescaletier/) { get; set; } | Ottiene o imposta le impostazioni del livello di scala cronologica inferiore della vista. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/) |
| [CustomBarStyles](../../aspose.tasks/ganttchartview/custombarstyles/) { get; } | Ottiene un elenco di stili di barra personalizzati specifici per attività della visualizzazione Diagramma di Gantt. [`GanttBarStyle`](../../aspose.tasks.visualization/ganttbarstyle/) . |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | Ottiene o imposta un filtro utilizzato in una vista singola. |
| [Gridlines](../../aspose.tasks/ganttchartview/gridlines/) { get; set; } | Ottiene o imposta un elenco di[`Gridlines`](./gridlines/) della vista Diagramma di Gantt. |
| [Group](../../aspose.tasks/view/group/) { get; set; } | Ottiene o imposta un gruppo della vista singola. |
| [HideRollupBarsWhenSummaryExpanded](../../aspose.tasks/ganttchartview/hiderollupbarswhensummaryexpanded/) { get; set; } | Ottiene o imposta un valore che indica se le barre di rollup saranno nascoste durante l'espansione dell'attività di riepilogo. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | Ottiene o imposta un valore che indica se Microsoft Project evidenzia il filtro per una singola vista. |
| [MiddleTimescaleTier](../../aspose.tasks/ganttchartview/middletimescaletier/) { get; set; } | Ottiene o imposta le impostazioni del livello medio della scala temporale della vista. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/) . |
| [Name](../../aspose.tasks/view/name/) { get; set; } | Ottiene o imposta il nome di un oggetto View. |
| [NonWorkingTimeColor](../../aspose.tasks/ganttchartview/nonworkingtimecolor/) { get; set; } | Ottiene o imposta il colore dell'orario non lavorativo. |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | Ottiene un'istanza di[`PageInfo`](../view/pageinfo/)classe. Rappresenta i dati di impostazione della pagina presenti nel formato di file mpp. |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | Ottiene l'elemento padre dell'oggetto View. Sola lettura[`Project`](../project/) . |
| [ProgressLines](../../aspose.tasks/ganttchartview/progresslines/) { get; set; } | Recupera o imposta le linee di avanzamento per la visualizzazione Diagramma di Gantt. [`ProgressLines`](./progresslines/) . |
| [RollUpGanttBars](../../aspose.tasks/ganttchartview/rollupganttbars/) { get; set; } | Ottiene o imposta un valore che indica se le barre del diagramma di Gantt devono essere raggruppate. |
| [Screen](../../aspose.tasks/view/screen/) { get; } | Ottiene il tipo di schermo per la visualizzazione singola. Sola lettura[`ViewScreen`](../viewscreen/) . |
| [ShowBarSplits](../../aspose.tasks/ganttchartview/showbarsplits/) { get; set; } | Ottiene o imposta un valore che indica se devono essere visualizzate le suddivisioni delle attività nel diagramma di Gantt. |
| [ShowDrawings](../../aspose.tasks/ganttchartview/showdrawings/) { get; set; } | Ottiene o imposta un valore che indica se i disegni nel diagramma di Gantt devono essere visualizzati. |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | Ottiene o imposta un valore che indica se Microsoft Project mostra il nome della singola visualizzazione negli elenchi a discesa Visualizza o Altre visualizzazioni nella barra multifunzione. |
| [Table](../../aspose.tasks/view/table/) { get; set; } | Ottiene o imposta una tabella della vista singola. |
| [TableTextStyles](../../aspose.tasks/ganttchartview/tabletextstyles/) { get; } | Ottiene un elenco di stili di testo tabella della visualizzazione Diagramma di Gantt. [`TableTextStyle`](../../aspose.tasks.visualization/tabletextstyle/) . |
| [TextStyles](../../aspose.tasks/ganttchartview/textstyles/) { get; set; } | Ottiene o imposta un elenco di[`TextStyle`](../../aspose.tasks.visualization/textstyle/) della vista Diagramma di Gantt. |
| [TimescaleSizePercentage](../../aspose.tasks/ganttchartview/timescalesizepercentage/) { get; set; } |  |
| [TopTimescaleTier](../../aspose.tasks/ganttchartview/toptimescaletier/) { get; set; } | Ottiene o imposta le impostazioni del livello di scala cronologica superiore della vista. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/) . |
| [Type](../../aspose.tasks/view/type/) { get; } | Ottiene il tipo di elemento nella visualizzazione singola, ad esempio attività o risorse. Sola lettura[`ItemType`](../itemtype/) . |
| [Uid](../../aspose.tasks/view/uid/) { get; } | Ottiene l'identificatore univoco di una vista. |
| [VisualObjectsPlacements](../../aspose.tasks/view/visualobjectsplacements/) { get; } | Ottiene una raccolta di oggetti che rappresentano il posizionamento e l'aspetto di[`OleObject`](../oleobject/) nella vista. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [CompareTo](../../aspose.tasks/view/compareto/)(View) | Confronta l'istanza corrente con un altro oggetto dello stesso tipo e restituisce un numero intero che indica se l'istanza corrente precede, segue o si trova nella stessa posizione nell'ordinamento dell'altro oggetto. |
| override [Equals](../../aspose.tasks/view/equals/)(object) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| override [GetHashCode](../../aspose.tasks/view/gethashcode/)() | Restituisce un valore di codice hash per l'istanza di[`Resource`](../resource/) classe. |

### Guarda anche

* class [View](../view/)
* spazio dei nomi [Aspose.Tasks](../../aspose.tasks/)
* assemblea [Aspose.Tasks](../../)


