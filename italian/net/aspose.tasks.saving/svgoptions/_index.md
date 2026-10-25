---
title: "Classe SvgOptions"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Saving.SvgOptions. Consente di specificare opzioni aggiuntive durante il rendering delle pagine del progetto in SVG"
type: docs
weight: 2230
url: /it/net/aspose.tasks.saving/svgoptions/
---
## SvgOptions class

Consente di specificare opzioni aggiuntive durante il rendering delle pagine del progetto in SVG.

```csharp
public class SvgOptions : SaveOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [SvgOptions](svgoptions/)() | Inizializza una nuova istanza della classe `SvgOptions` che può essere utilizzata per salvare il progetto in formato SVG. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | Ottiene o imposta l'elenco delle istanze della classe [`BarStyle`](../../aspose.tasks.visualization/barstyle/) che appaiono nella vista del progetto. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | Ottiene o imposta la dimensione della pagina personalizzata in punti (1 punto = 1/72 di pollice). |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | Ottiene o imposta un valore che indica se il tempo non lavorativo deve essere disegnato (Il valore predefinito è TRUE). |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | Ottiene o imposta una data a cui terminare il rendering. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | Ottiene o imposta un valore che indica se l'altezza della riga deve essere aumentata per adattarsi al contenuto. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | Ottiene o imposta un elenco di [`Gridline`](../../aspose.tasks.visualization/gridline/) che appaiono nella vista del progetto. |
| [IsPortrait](../../aspose.tasks.saving/saveoptions/isportrait/) { get; set; } | Ottiene o imposta un valore che indica se l'orientamento della pagina è verticale; restituisce false se l'orientamento della pagina è orizzontale. |
| [LegendDrawingOptions](../../aspose.tasks.saving/saveoptions/legenddrawingoptions/) { get; set; } | Ottiene o imposta un valore che definisce come renderizzare una legenda. Il valore predefinito è LegendDrawingOptions.OnEveryPage. |
| [LegendItems](../../aspose.tasks.saving/saveoptions/legenditems/) { get; set; } | Ottiene o imposta un array di PageLegendItem che definisce quali barre devono essere renderizzate nella legenda della pagina. Se null, vengono renderizzati gli elementi predefiniti. |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | Ottiene o imposta un valore che indica se le attività critiche devono essere visualizzate in colore rosso (Il valore predefinito è FALSE). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | Ottiene o imposta il colore del tempo non lavorativo. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | Ottiene o imposta il numero di pagine del progetto. |
| [PageSavingCallback](../../aspose.tasks.saving/svgoptions/pagesavingcallback/) { get; set; } | Ottiene o imposta una callback di implementazione definita dall'utente che viene utilizzata per ottenere uno stream di output per ogni pagina renderizzata. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | Ottiene o imposta la dimensione della pagina da renderizzare (Il valore predefinito è PageSize.A4). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | Ottiene o imposta il [`PresentationFormat`](../saveoptions/presentationformat/) in cui il documento sarà salvato. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | Ottiene o imposta un valore che indica se un progetto deve essere renderizzato su una singola pagina quando il progetto è salvato in formato grafico. La dimensione della pagina sarà modificata in modo che il progetto renderizzato possa adattarsi a una pagina. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | Ottiene o imposta un valore che indica se le sottoattività sulla barra dell'attività di riepilogo devono essere contrassegnate. Per le sottoattività, il campo Rollup indica se le informazioni sulle barre Gantt delle sottoattività verranno aggregate nella barra dell'attività di riepilogo. Per le attività di riepilogo, il campo Rollup indica se la barra dell'attività di riepilogo visualizza le barre aggregate. È necessario impostare il campo Rollup per le attività di riepilogo su Yes affinché le sottoattività vengano aggregate. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Ottiene o imposta il formato in cui il documento verrà salvato se viene utilizzato questo oggetto di opzioni di salvataggio. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | Ottiene o imposta la data da cui iniziare il rendering. |
| [TaskLinkDrawingCallback](../../aspose.tasks.saving/saveoptions/tasklinkdrawingcallback/) { get; set; } | Ottiene o imposta una callback che può essere usata per personalizzare alcuni aspetti del rendering dei collegamenti tra attività. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Ottiene o imposta il comparatore per ordinare le attività nel diagramma di Gantt e nella tabella delle attività. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Ottiene o imposta la condizione utilizzata per filtrare le attività visualizzate nei diagrammi Gantt, nella tabella delle attività e nell'utilizzo delle attività. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | Ottiene o imposta l'elenco degli stili di testo applicati durante il rendering di una vista di progetto. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | Ottiene o imposta il valore [`Timescale`](../saveoptions/timescale/) utilizzato per controllare come la scala temporale (se presente) viene renderizzata quando il progetto viene salvato in formato grafico. |
| [TimescaleFitBehavior](../../aspose.tasks.saving/saveoptions/timescalefitbehavior/) { get; set; } | Ottiene o imposta un comportamento che definisce come allineare l'estremità destra della scala temporale con il bordo della pagina. |
| override [UseGradientBrush](../../aspose.tasks.saving/svgoptions/usegradientbrush/) { get; set; } | Determina se utilizzare un pennello gradiente durante il rendering del layout del progetto. Attualmente l'uso del pennello gradiente non è supportato per il rendering in SVG. |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | Ottiene o imposta un elenco delle colonne della vista da renderizzare ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)). Se non impostato, vengono renderizzati solo gli ID delle attività, i nomi delle attività, l'inizio e la fine. Se entrambe le proprietà View e [`ViewSettings`](../saveoptions/viewsettings/) sono impostate, le colonne da View sovrascrivono quelle da ViewSettings. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | Ottiene o imposta una vista ([`View`](../saveoptions/view/)) da renderizzare. È possibile utilizzare questa opzione per specificare esplicitamente quale vista deve essere salvata nei formati PDF, HTML o immagine. Se questa proprietà è impostata, la proprietà [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) viene ignorata quando il progetto viene salvato. La vista deve provenire da una delle seguenti schermate (([`Screen`](../../aspose.tasks/view/screen/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage). |

## Esempi

Mostra come salvare il progetto come file SVG.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
SaveOptions options = new SvgOptions
                        {
                            // imposta il <see cref=\"P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat\" /> in cui il documento sarà salvato
                            PresentationFormat = PresentationFormat.GanttChart,

                            // imposta un valore che indica se l'altezza della riga deve essere aumentata per adattarsi al contenuto
                            FitContent = true,

                            // imposta il periodo di tempo minimo da renderizzare. Il valore predefinito è <see cref=\"P:Aspose.Tasks.Saving.SaveOptions.Timescale\">Days</see>
                            Timescale = Timescale.ThirdsOfMonths,

                            // determina se utilizzare un pennello gradiente durante il rendering del layout del progetto
                            // Attualmente l'uso del pennello gradiente non è supportato per il rendering in SVG.
                            // UseGradientBrush = true
                        };
project.Save(OutDir + "UseSvgOptions_out.svg", options);
```

### Vedi anche

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


