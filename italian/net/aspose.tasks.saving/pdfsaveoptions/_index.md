---
title: PdfSaveOptions
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: Consente di specificare opzioni aggiuntive durante il rendering di pagine di progetto in PDF.
type: docs
weight: 1850
url: /it/net/aspose.tasks.saving/pdfsaveoptions/
---
## PdfSaveOptions class

Consente di specificare opzioni aggiuntive durante il rendering di pagine di progetto in PDF.

```csharp
public class PdfSaveOptions : SaveOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions)() | Inizializza una nuova istanza di[`PdfSaveOptions`](../pdfsaveoptions)classe che può essere utilizzata per salvare un documento in[`PDF`](../savefileformat) formato. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles) { get; set; } | Ottiene o imposta l'elenco delle istanze di[`BarStyle`](../../aspose.tasks.visualization/barstyle) classe che appare nella vista progetto. |
| [Compliance](../../aspose.tasks.saving/pdfsaveoptions/compliance) { get; set; } | Ottiene o imposta un livello di conformità desiderato per il documento PDF generato. L'impostazione predefinita èPdf15 . |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize) { get; set; } | Ottiene o imposta la dimensione della pagina personalizzata in punti (1 punto = 1/72 di pollice). |
| [DefaultFontName](../../aspose.tasks.saving/pdfsaveoptions/defaultfontname) { get; set; } | Ottiene o imposta il carattere predefinito per il rendering. |
| [DigitalSignatureDetails](../../aspose.tasks.saving/pdfsaveoptions/digitalsignaturedetails) { get; set; } | Ottiene o imposta i dettagli di una firma digitale. Se non è impostato, non verrà eseguita alcuna firma. |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime) { get; set; } | Ottiene o imposta un valore che indica se l'orario non lavorativo deve essere disegnato (il valore predefinito è TRUE). |
| [EncryptionDetails](../../aspose.tasks.saving/pdfsaveoptions/encryptiondetails) { get; set; } | Ottiene o imposta i dettagli di crittografia. Se non è impostato, non verrà eseguita alcuna crittografia. |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate) { get; set; } | Ottiene o imposta una data in cui terminare il rendering. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent) { get; set; } | Ottiene o imposta un valore che indica se l'altezza della riga deve essere aumentata per adattarla al contenuto. |
| [FontResolveCallback](../../aspose.tasks.saving/pdfsaveoptions/fontresolvecallback) { get; set; } | Ottiene o imposta un callback che può essere utilizzato per personalizzare i caratteri risolti. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines) { get; set; } | Ottiene o imposta un elenco di[`Gridline`](../../aspose.tasks.visualization/gridline) che appaiono nella vista progetto. |
| [LegendOnEachPage](../../aspose.tasks.saving/saveoptions/legendoneachpage) { get; set; } | Ottiene o imposta un valore che indica se la legenda deve essere visualizzata su ciascuna pagina (il valore predefinito è TRUE). |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks) { get; set; } | Ottiene o imposta un valore che indica se le attività critiche devono essere visualizzate in rosso (il valore predefinito è FALSE). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor) { get; set; } | Ottiene o imposta il colore dell'orario non lavorativo. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount) { get; } | Ottiene o imposta il numero di pagine del progetto. |
| [Pages](../../aspose.tasks.saving/pdfsaveoptions/pages) { get; set; } | Ottiene o imposta l'elenco dei numeri di pagina da salvare quando si salva il layout del progetto in file separati. Tutte le pagine verranno salvate se questo elenco è vuoto. |
| [PageSavingCallback](../../aspose.tasks.saving/pdfsaveoptions/pagesavingcallback) { get; set; } | Ottiene o imposta un callback definito dall'utente che viene utilizzato per ottenere un flusso di output per ogni pagina sottoposta a rendering. È applicabile quando[`SaveToSeparateFiles`](./savetoseparatefiles) viene utilizzata l'opzione. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize) { get; set; } | Ottiene o imposta la dimensione della pagina di cui eseguire il rendering (il valore predefinito è PageSize.A4). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat) { get; set; } | Ottiene o imposta il[`PresentationFormat`](../saveoptions/presentationformat) in cui verrà salvato il documento. |
| [ReduceFooterGap](../../aspose.tasks.saving/pdfsaveoptions/reducefootergap) { get; set; } | Ottiene o imposta un valore che indica se è necessario ridurre lo spazio tra l'ultima attività e il piè di pagina. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage) { get; set; } | Ottiene o imposta un valore che indica se è necessario eseguire il rendering di un progetto su una singola pagina quando il progetto viene salvato in formato grafico. Le dimensioni della pagina verranno modificate in modo che il progetto renderizzato possa adattarsi a una pagina. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars) { get; set; } | Ottiene o imposta un valore che indica se le attività secondarie sulla barra delle attività di riepilogo devono essere contrassegnate. Per le attività secondarie, il campo Riepiloga indica se le informazioni sulle barre di Gantt delle attività secondarie verranno riportate nella barra delle attività di riepilogo. Per le attività di riepilogo, il Riepilogo campo indica se la barra delle attività di riepilogo visualizza le barre arrotolate. È necessario che il campo Riepilogo per le attività di riepilogo sia impostato su Sì affinché tutte le attività secondarie possano essere ripristinate. |
| [SaveFormat](../../aspose.tasks.saving/saveoptions/saveformat) { get; } | Ottiene o imposta il formato in cui verrà salvato il documento se viene utilizzato questo oggetto delle opzioni di salvataggio. |
| [SaveToSeparateFiles](../../aspose.tasks.saving/pdfsaveoptions/savetoseparatefiles) { get; set; } | Ottiene o imposta un valore che indica se salvare le pagine del progetto in file separati. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate) { get; set; } | Ottiene o imposta la data da cui iniziare il rendering. |
| [TasksComparer](../../aspose.tasks.saving/saveoptions/taskscomparer) { get; set; } | Ottiene o imposta il comparatore per ordinare le attività sul diagramma di Gantt e sul diagramma del foglio attività. |
| [TasksFilter](../../aspose.tasks.saving/saveoptions/tasksfilter) { get; set; } | Ottiene o imposta la condizione utilizzata per filtrare le attività di cui viene eseguito il rendering su Gantt, Foglio attività e Grafici di utilizzo attività. |
| [TextCompression](../../aspose.tasks.saving/pdfsaveoptions/textcompression) { get; set; } | Ottiene o imposta un tipo di compressione da utilizzare per tutti i flussi di contenuto eccetto le immagini. L'impostazione predefinita èFlate . |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles) { get; set; } | Ottiene o imposta l'elenco delle istanze di[`TextStyle`](../../aspose.tasks.visualization/textstyle) classe che appare nella vista progetto. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale) { get; set; } | Ottiene o imposta il[`Timescale`](../saveoptions/timescale) valore che viene utilizzato per controllare la modalità di rendering della scala temporale (se presente) quando il progetto viene salvato in formato grafico. |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush) { get; set; } | Ottiene o imposta un valore che indica se utilizzare il pennello sfumatura durante il rendering del diagramma di Gantt. |
| [UseProjectDefaultFont](../../aspose.tasks.saving/pdfsaveoptions/useprojectdefaultfont) { get; set; } | Ottiene o imposta un valore che indica se il carattere predefinito deve essere utilizzato per il rendering. |
| [View](../../aspose.tasks.saving/saveoptions/view) { get; set; } | Ottiene o imposta un elenco delle colonne della vista di cui eseguire il rendering ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn) ). Se non è impostato, vengono visualizzati solo gli ID attività, i nomi delle attività, l'inizio e la fine. Se sia Visualizza che[`ViewSettings`](../saveoptions/viewsettings) le proprietà sono impostate, le colonne di View hanno la precedenza sulle colonne di ViewSettings. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings) { get; set; } | Ottiene o imposta una vista ([`View`](../saveoptions/view) per rendere. È possibile utilizzare queste opzioni per specificare in modo esplicito quale vista deve essere salvata nei formati PDF, HTML o immagine. Se questa proprietà è impostata,[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat) la proprietà viene ignorata quando il progetto viene salvato. La vista dovrebbe provenire da una delle seguenti schermate (([`Screen`](../../aspose.tasks/view/screen) )): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |

### Guarda anche

* class [SaveOptions](../saveoptions)
* spazio dei nomi [Aspose.Tasks.Saving](../../aspose.tasks.saving)
* assemblea [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->