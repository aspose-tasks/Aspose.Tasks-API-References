---
title: "Classe ImageSaveOptions"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Saving.ImageSaveOptions. Consente di specificare opzioni aggiuntive durante il rendering delle pagine del progetto in immagini"
type: docs
weight: 2030
url: /it/net/aspose.tasks.saving/imagesaveoptions/
---
## ImageSaveOptions class

Consente di specificare opzioni aggiuntive durante il rendering delle pagine del progetto in immagini.

```csharp
public class ImageSaveOptions : SaveOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [ImageSaveOptions](imagesaveoptions/)(SaveFileFormat) | Inizializza una nuova istanza della classe `ImageSaveOptions` che può essere utilizzata per salvare le immagini renderizzate nei formati TIFF, PNG, BMP o JPEG. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | Ottiene o imposta l'elenco delle istanze della classe [`BarStyle`](../../aspose.tasks.visualization/barstyle/) che appaiono nella vista del progetto. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | Ottiene o imposta la dimensione della pagina personalizzata in punti (1 punto = 1/72 di pollice). |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | Ottiene o imposta un valore che indica se il tempo non lavorativo deve essere disegnato (Il valore predefinito è TRUE). |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | Ottiene o imposta una data a cui terminare il rendering. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | Ottiene o imposta un valore che indica se l'altezza della riga deve essere aumentata per adattarsi al contenuto. |
| [FontSettings](../../aspose.tasks.saving/imagesaveoptions/fontsettings/) { get; } | Specifica le impostazioni del font utilizzate durante il rendering della vista del progetto. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | Ottiene o imposta un elenco di [`Gridline`](../../aspose.tasks.visualization/gridline/) che appaiono nella vista del progetto. |
| [HorizontalResolution](../../aspose.tasks.saving/imagesaveoptions/horizontalresolution/) { get; set; } | Ottiene o imposta la risoluzione orizzontale in dpi. |
| [IsPortrait](../../aspose.tasks.saving/saveoptions/isportrait/) { get; set; } | Ottiene o imposta un valore che indica se l'orientamento della pagina è verticale; restituisce false se l'orientamento della pagina è orizzontale. |
| [JpegQuality](../../aspose.tasks.saving/imagesaveoptions/jpegquality/) { get; set; } | Ottiene o imposta la qualità JPEG. L'intervallo di valori consentito è 0..100. |
| [LegendDrawingOptions](../../aspose.tasks.saving/saveoptions/legenddrawingoptions/) { get; set; } | Ottiene o imposta un valore che definisce come renderizzare una legenda. Il valore predefinito è LegendDrawingOptions.OnEveryPage. |
| [LegendItems](../../aspose.tasks.saving/saveoptions/legenditems/) { get; set; } | Ottiene o imposta un array di PageLegendItem che definisce quali barre devono essere renderizzate nella legenda della pagina. Se null, vengono renderizzati gli elementi predefiniti. |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | Ottiene o imposta un valore che indica se le attività critiche devono essere visualizzate in colore rosso (Il valore predefinito è FALSE). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | Ottiene o imposta il colore del tempo non lavorativo. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | Ottiene o imposta il numero di pagine del progetto. |
| [Pages](../../aspose.tasks.saving/imagesaveoptions/pages/) { get; set; } | Ottiene o imposta un elenco di numeri di pagina da salvare quando il layout del progetto viene salvato in file separati. Tutte le pagine verranno salvate se questo elenco è vuoto. |
| [PageSavingCallback](../../aspose.tasks.saving/imagesaveoptions/pagesavingcallback/) { get; set; } | Ottiene o imposta un callback definito dall'utente che viene utilizzato per ottenere uno stream di output per ogni pagina renderizzata. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | Ottiene o imposta la dimensione della pagina da renderizzare (Il valore predefinito è PageSize.A4). |
| [PixelFormat](../../aspose.tasks.saving/imagesaveoptions/pixelformat/) { get; set; } | Ottiene o imposta il formato dei dati di colore per ogni pixel nell'immagine. |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | Ottiene o imposta il [`PresentationFormat`](../saveoptions/presentationformat/) in cui il documento sarà salvato. |
| [ReduceFooterGap](../../aspose.tasks.saving/imagesaveoptions/reducefootergap/) { get; set; } | Ottiene o imposta un valore che indica se lo spazio tra l'ultima attività e il piè di pagina deve essere ridotto. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | Ottiene o imposta un valore che indica se un progetto deve essere renderizzato su una singola pagina quando il progetto è salvato in formato grafico. La dimensione della pagina sarà modificata in modo che il progetto renderizzato possa adattarsi a una pagina. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | Ottiene o imposta un valore che indica se le sottoattività sulla barra dell'attività di riepilogo devono essere contrassegnate. Per le sottoattività, il campo Rollup indica se le informazioni sulle barre Gantt delle sottoattività verranno aggregate nella barra dell'attività di riepilogo. Per le attività di riepilogo, il campo Rollup indica se la barra dell'attività di riepilogo visualizza le barre aggregate. È necessario impostare il campo Rollup per le attività di riepilogo su Yes affinché le sottoattività vengano aggregate. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Ottiene o imposta il formato in cui il documento verrà salvato se viene utilizzato questo oggetto di opzioni di salvataggio. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | Ottiene o imposta la data da cui iniziare il rendering. |
| [TaskLinkDrawingCallback](../../aspose.tasks.saving/saveoptions/tasklinkdrawingcallback/) { get; set; } | Ottiene o imposta una callback che può essere usata per personalizzare alcuni aspetti del rendering dei collegamenti tra attività. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Ottiene o imposta il comparatore per ordinare le attività nel diagramma di Gantt e nella tabella delle attività. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Ottiene o imposta la condizione utilizzata per filtrare le attività visualizzate nei diagrammi Gantt, nella tabella delle attività e nell'utilizzo delle attività. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | Ottiene o imposta l'elenco degli stili di testo applicati durante il rendering di una vista di progetto. |
| [TiffCompression](../../aspose.tasks.saving/imagesaveoptions/tiffcompression/) { get; set; } | Ottiene o imposta il tipo di compressione da applicare quando le immagini generate vengono salvate nel formato TIFF. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | Ottiene o imposta il valore [`Timescale`](../saveoptions/timescale/) utilizzato per controllare come la scala temporale (se presente) viene renderizzata quando il progetto viene salvato in formato grafico. |
| [TimescaleFitBehavior](../../aspose.tasks.saving/saveoptions/timescalefitbehavior/) { get; set; } | Ottiene o imposta un comportamento che definisce come allineare l'estremità destra della scala temporale con il bordo della pagina. |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush/) { get; set; } | Ottiene o imposta un valore che indica se deve essere utilizzato un pennello gradiente durante il rendering del diagramma di Gantt. |
| [VerticalResolution](../../aspose.tasks.saving/imagesaveoptions/verticalresolution/) { get; set; } | Ottiene o imposta la risoluzione verticale in dpi. |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | Ottiene o imposta un elenco delle colonne della vista da renderizzare ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)). Se non impostato, vengono renderizzati solo gli ID delle attività, i nomi delle attività, l'inizio e la fine. Se entrambe le proprietà View e [`ViewSettings`](../saveoptions/viewsettings/) sono impostate, le colonne da View sovrascrivono quelle da ViewSettings. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | Ottiene o imposta una vista ([`View`](../saveoptions/view/)) da renderizzare. È possibile utilizzare questa opzione per specificare esplicitamente quale vista deve essere salvata nei formati PDF, HTML o immagine. Se questa proprietà è impostata, la proprietà [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) viene ignorata quando il progetto viene salvato. La vista deve provenire da una delle seguenti schermate (([`Screen`](../../aspose.tasks/view/screen/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage). |

## Esempi

Mostra come salvare il progetto in uno stream come immagine.

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var options = new ImageSaveOptions(SaveFileFormat.Png);

    // utilizzando ImageSaveOptions salviamo il progetto in formato immagine
    project.Save(stream, options);
}
```

### Vedi anche

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


