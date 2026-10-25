---
title: "Classe PdfSaveOptions"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Saving.PdfSaveOptions. Consente di specificare opzioni aggiuntive durante il rendering delle pagine del progetto in PDF"
type: docs
weight: 2130
url: /it/net/aspose.tasks.saving/pdfsaveoptions/
---
## PdfSaveOptions class

Consente di specificare opzioni aggiuntive durante il rendering delle pagine del progetto in PDF.

```csharp
public class PdfSaveOptions : SaveOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions/)() | Inizializza una nuova istanza della classe `PdfSaveOptions` che può essere utilizzata per salvare un documento nel formato [`PDF`](../savefileformat/). |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | Ottiene o imposta l'elenco delle istanze della classe [`BarStyle`](../../aspose.tasks.visualization/barstyle/) che appaiono nella vista del progetto. |
| [Compliance](../../aspose.tasks.saving/pdfsaveoptions/compliance/) { get; set; } | Ottiene o imposta il livello di conformità desiderato per il documento PDF generato. Il valore predefinito è Pdf15. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | Ottiene o imposta la dimensione della pagina personalizzata in punti (1 punto = 1/72 di pollice). |
| [DigitalSignatureDetails](../../aspose.tasks.saving/pdfsaveoptions/digitalsignaturedetails/) { get; set; } | Ottiene o imposta i dettagli della firma digitale. Se non impostato, non verrà eseguita alcuna firma. |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | Ottiene o imposta un valore che indica se il tempo non lavorativo deve essere disegnato (Il valore predefinito è TRUE). |
| [EncryptionDetails](../../aspose.tasks.saving/pdfsaveoptions/encryptiondetails/) { get; set; } | Ottiene o imposta i dettagli della crittografia. Se non impostato, non verrà eseguita alcuna crittografia. |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | Ottiene o imposta una data a cui terminare il rendering. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | Ottiene o imposta un valore che indica se l'altezza della riga deve essere aumentata per adattarsi al contenuto. |
| [FontSettings](../../aspose.tasks.saving/pdfsaveoptions/fontsettings/) { get; } | Specifica le impostazioni del font utilizzate durante il rendering della vista del progetto. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | Ottiene o imposta un elenco di [`Gridline`](../../aspose.tasks.visualization/gridline/) che appaiono nella vista del progetto. |
| [IsPortrait](../../aspose.tasks.saving/saveoptions/isportrait/) { get; set; } | Ottiene o imposta un valore che indica se l'orientamento della pagina è verticale; restituisce false se l'orientamento della pagina è orizzontale. |
| [LegendDrawingOptions](../../aspose.tasks.saving/saveoptions/legenddrawingoptions/) { get; set; } | Ottiene o imposta un valore che definisce come renderizzare una legenda. Il valore predefinito è LegendDrawingOptions.OnEveryPage. |
| [LegendItems](../../aspose.tasks.saving/saveoptions/legenditems/) { get; set; } | Ottiene o imposta un array di PageLegendItem che definisce quali barre devono essere renderizzate nella legenda della pagina. Se null, vengono renderizzati gli elementi predefiniti. |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | Ottiene o imposta un valore che indica se le attività critiche devono essere visualizzate in colore rosso (Il valore predefinito è FALSE). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | Ottiene o imposta il colore del tempo non lavorativo. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | Ottiene o imposta il numero di pagine del progetto. |
| [Pages](../../aspose.tasks.saving/pdfsaveoptions/pages/) { get; set; } | Ottiene o imposta l'elenco dei numeri di pagina da salvare quando il layout del progetto viene salvato in file separati. Tutte le pagine verranno salvate se questo elenco è vuoto. |
| [PageSavingCallback](../../aspose.tasks.saving/pdfsaveoptions/pagesavingcallback/) { get; set; } | Ottiene o imposta una callback definita dall'utente che viene utilizzata per ottenere uno stream di output per ogni pagina renderizzata. È applicabile quando viene usata l'opzione [`SaveToSeparateFiles`](./savetoseparatefiles/). |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | Ottiene o imposta la dimensione della pagina da renderizzare (Il valore predefinito è PageSize.A4). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | Ottiene o imposta il [`PresentationFormat`](../saveoptions/presentationformat/) in cui il documento sarà salvato. |
| [ReduceFooterGap](../../aspose.tasks.saving/pdfsaveoptions/reducefootergap/) { get; set; } | Ottiene o imposta un valore che indica se lo spazio tra l'ultima attività e il piè di pagina deve essere ridotto. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | Ottiene o imposta un valore che indica se un progetto deve essere renderizzato su una singola pagina quando il progetto è salvato in formato grafico. La dimensione della pagina sarà modificata in modo che il progetto renderizzato possa adattarsi a una pagina. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | Ottiene o imposta un valore che indica se le sottoattività sulla barra dell'attività di riepilogo devono essere contrassegnate. Per le sottoattività, il campo Rollup indica se le informazioni sulle barre Gantt delle sottoattività verranno aggregate nella barra dell'attività di riepilogo. Per le attività di riepilogo, il campo Rollup indica se la barra dell'attività di riepilogo visualizza le barre aggregate. È necessario impostare il campo Rollup per le attività di riepilogo su Yes affinché le sottoattività vengano aggregate. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Ottiene o imposta il formato in cui il documento verrà salvato se viene utilizzato questo oggetto di opzioni di salvataggio. |
| [SaveToSeparateFiles](../../aspose.tasks.saving/pdfsaveoptions/savetoseparatefiles/) { get; set; } | Ottiene o imposta un valore che indica se salvare le pagine del progetto in file separati. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | Ottiene o imposta la data da cui iniziare il rendering. |
| [TaskLinkDrawingCallback](../../aspose.tasks.saving/saveoptions/tasklinkdrawingcallback/) { get; set; } | Ottiene o imposta una callback che può essere usata per personalizzare alcuni aspetti del rendering dei collegamenti tra attività. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Ottiene o imposta il comparatore per ordinare le attività nel diagramma di Gantt e nella tabella delle attività. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Ottiene o imposta la condizione utilizzata per filtrare le attività visualizzate nei diagrammi Gantt, nella tabella delle attività e nell'utilizzo delle attività. |
| [TextCompression](../../aspose.tasks.saving/pdfsaveoptions/textcompression/) { get; set; } | Ottiene o imposta il tipo di compressione da utilizzare per tutti i flussi di contenuto eccetto le immagini. Il valore predefinito è Flate. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | Ottiene o imposta l'elenco degli stili di testo applicati durante il rendering di una vista di progetto. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | Ottiene o imposta il valore [`Timescale`](../saveoptions/timescale/) utilizzato per controllare come la scala temporale (se presente) viene renderizzata quando il progetto viene salvato in formato grafico. |
| [TimescaleFitBehavior](../../aspose.tasks.saving/saveoptions/timescalefitbehavior/) { get; set; } | Ottiene o imposta un comportamento che definisce come allineare l'estremità destra della scala temporale con il bordo della pagina. |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush/) { get; set; } | Ottiene o imposta un valore che indica se deve essere utilizzato un pennello gradiente durante il rendering del diagramma di Gantt. |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | Ottiene o imposta un elenco delle colonne della vista da renderizzare ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)). Se non impostato, vengono renderizzati solo gli ID delle attività, i nomi delle attività, l'inizio e la fine. Se entrambe le proprietà View e [`ViewSettings`](../saveoptions/viewsettings/) sono impostate, le colonne da View sovrascrivono quelle da ViewSettings. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | Ottiene o imposta una vista ([`View`](../saveoptions/view/)) da renderizzare. È possibile utilizzare questa opzione per specificare esplicitamente quale vista deve essere salvata nei formati PDF, HTML o immagine. Se questa proprietà è impostata, la proprietà [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) viene ignorata quando il progetto viene salvato. La vista deve provenire da una delle seguenti schermate (([`Screen`](../../aspose.tasks/view/screen/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage). |

## Esempi

Mostra come salvare le pagine selezionate di un progetto in un file PDF.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");
var options = new PdfSaveOptions();
options.RenderToSinglePage = false;
options.Pages = new List<int>();

// verifichiamo il numero di pagine che possono essere esportate
Console.WriteLine("Page Count: " + options.PageCount);

options.Pages.Add(1);
options.Pages.Add(4);
project.Save(OutDir + "SaveToMultiplePDFFiles_out.pdf", options);
```

### Vedi anche

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


