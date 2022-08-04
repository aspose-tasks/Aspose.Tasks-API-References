---
title: XlsxOptions
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: Consente di specificare opzioni aggiuntive durante il rendering di pagine di progetto su XLSX.
type: docs
weight: 1970
url: /it/net/aspose.tasks.saving/xlsxoptions/
---
## XlsxOptions class

Consente di specificare opzioni aggiuntive durante il rendering di pagine di progetto su XLSX.

```csharp
public class XlsxOptions : SaveOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [XlsxOptions](xlsxoptions)() | Inizializza una nuova istanza di[`XlsxOptions`](../xlsxoptions)classe che può essere utilizzata per salvare il progetto in formato XLSX. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AssignmentView](../../aspose.tasks.saving/xlsxoptions/assignmentview) { get; set; } | Ottiene o imposta un elenco delle colonne della vista assegnazioni di cui eseguire il rendering ([`AssignmentViewColumn`](../../aspose.tasks.visualization/assignmentviewcolumn) ). |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles) { get; set; } | Ottiene o imposta l'elenco delle istanze di[`BarStyle`](../../aspose.tasks.visualization/barstyle) classe che appare nella vista progetto. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize) { get; set; } | Ottiene o imposta la dimensione della pagina personalizzata in punti (1 punto = 1/72 di pollice). |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime) { get; set; } | Ottiene o imposta un valore che indica se l'orario non lavorativo deve essere disegnato (il valore predefinito è TRUE). |
| [Encoding](../../aspose.tasks.saving/xlsxoptions/encoding) { get; set; } | Ottiene o imposta la codifica del file XLSX risultante. Il valore predefinito èUTF8 . |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate) { get; set; } | Ottiene o imposta una data in cui terminare il rendering. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent) { get; set; } | Ottiene o imposta un valore che indica se l'altezza della riga deve essere aumentata per adattarla al contenuto. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines) { get; set; } | Ottiene o imposta un elenco di[`Gridline`](../../aspose.tasks.visualization/gridline) che appaiono nella vista progetto. |
| [LegendOnEachPage](../../aspose.tasks.saving/saveoptions/legendoneachpage) { get; set; } | Ottiene o imposta un valore che indica se la legenda deve essere visualizzata su ciascuna pagina (il valore predefinito è TRUE). |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks) { get; set; } | Ottiene o imposta un valore che indica se le attività critiche devono essere visualizzate in rosso (il valore predefinito è FALSE). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor) { get; set; } | Ottiene o imposta il colore dell'orario non lavorativo. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount) { get; } | Ottiene o imposta il numero di pagine del progetto. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize) { get; set; } | Ottiene o imposta la dimensione della pagina di cui eseguire il rendering (il valore predefinito è PageSize.A4). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat) { get; set; } | Ottiene o imposta il[`PresentationFormat`](../saveoptions/presentationformat) in cui verrà salvato il documento. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage) { get; set; } | Ottiene o imposta un valore che indica se è necessario eseguire il rendering di un progetto su una singola pagina quando il progetto viene salvato in formato grafico. Le dimensioni della pagina verranno modificate in modo che il progetto renderizzato possa adattarsi a una pagina. |
| [ResourceView](../../aspose.tasks.saving/xlsxoptions/resourceview) { get; set; } | Ottiene o imposta un elenco delle colonne della visualizzazione delle risorse di cui eseguire il rendering ([`ResourceViewColumn`](../../aspose.tasks.visualization/resourceviewcolumn) ). |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars) { get; set; } | Ottiene o imposta un valore che indica se le attività secondarie sulla barra delle attività di riepilogo devono essere contrassegnate. Per le attività secondarie, il campo Riepiloga indica se le informazioni sulle barre di Gantt delle attività secondarie verranno riportate nella barra delle attività di riepilogo. Per le attività di riepilogo, il Riepilogo campo indica se la barra delle attività di riepilogo visualizza le barre arrotolate. È necessario che il campo Riepilogo per le attività di riepilogo sia impostato su Sì affinché tutte le attività secondarie possano essere ripristinate. |
| [SaveFormat](../../aspose.tasks.saving/saveoptions/saveformat) { get; } | Ottiene o imposta il formato in cui verrà salvato il documento se viene utilizzato questo oggetto delle opzioni di salvataggio. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate) { get; set; } | Ottiene o imposta la data da cui iniziare il rendering. |
| [TasksComparer](../../aspose.tasks.saving/saveoptions/taskscomparer) { get; set; } | Ottiene o imposta il comparatore per ordinare le attività sul diagramma di Gantt e sul diagramma del foglio attività. |
| [TasksFilter](../../aspose.tasks.saving/saveoptions/tasksfilter) { get; set; } | Ottiene o imposta la condizione utilizzata per filtrare le attività di cui viene eseguito il rendering su Gantt, Foglio attività e Grafici di utilizzo attività. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles) { get; set; } | Ottiene o imposta l'elenco delle istanze di[`TextStyle`](../../aspose.tasks.visualization/textstyle) classe che appare nella vista progetto. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale) { get; set; } | Ottiene o imposta il[`Timescale`](../saveoptions/timescale) valore che viene utilizzato per controllare la modalità di rendering della scala temporale (se presente) quando il progetto viene salvato in formato grafico. |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush) { get; set; } | Ottiene o imposta un valore che indica se utilizzare il pennello sfumatura durante il rendering del diagramma di Gantt. |
| [View](../../aspose.tasks.saving/saveoptions/view) { get; set; } | Ottiene o imposta un elenco delle colonne della vista di cui eseguire il rendering ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn) ). Se non è impostato, vengono visualizzati solo gli ID attività, i nomi delle attività, l'inizio e la fine. Se sia Visualizza che[`ViewSettings`](../saveoptions/viewsettings) le proprietà sono impostate, le colonne di View hanno la precedenza sulle colonne di ViewSettings. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings) { get; set; } | Ottiene o imposta una vista ([`View`](../saveoptions/view) per rendere. È possibile utilizzare queste opzioni per specificare in modo esplicito quale vista deve essere salvata nei formati PDF, HTML o immagine. Se questa proprietà è impostata,[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat) la proprietà viene ignorata quando il progetto viene salvato. La vista dovrebbe provenire da una delle seguenti schermate (([`Screen`](../../aspose.tasks/view/screen) )): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |

### Guarda anche

* class [SaveOptions](../saveoptions)
* spazio dei nomi [Aspose.Tasks.Saving](../../aspose.tasks.saving)
* assemblea [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
