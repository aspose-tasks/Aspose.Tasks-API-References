---
title: Class XamlOptions
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: Aspose.Tasks.Saving.XamlOptions classe. /// Consente di specificare opzioni aggiuntive durante il rendering delle pagine del progetto in XAML.
type: docs
weight: 1970
url: /it/net/aspose.tasks.saving/xamloptions/
---
## XamlOptions class

/// Consente di specificare opzioni aggiuntive durante il rendering delle pagine del progetto in XAML.

```csharp
public class XamlOptions : SaveOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [XamlOptions](xamloptions/)() | Inizializza una nuova istanza di`XamlOptions` classe che può essere utilizzata per salvare il progetto in formato XAML. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | Ottiene o imposta l'elenco delle istanze di[`BarStyle`](../../aspose.tasks.visualization/barstyle/) classe che appare nella vista del progetto. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | Ottiene o imposta la dimensione della pagina personalizzata in punti (1 punto = 1/72 di pollice). |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | Ottiene o imposta un valore che indica se deve essere disegnato l'orario non lavorativo (il valore predefinito è TRUE). |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | Ottiene o imposta una data in cui terminare il rendering. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | Ottiene o imposta un valore che indica se l'altezza della riga deve essere aumentata per adattarla al suo contenuto. |
| [FitTimescaleToEndOfPage](../../aspose.tasks.saving/saveoptions/fittimescaletoendofpage/) { get; set; } | Ottiene o imposta se il rendering di una sezione del calendario di una vista deve essere eseguito alla fine (lato destro) dell'ultima pagina. Se il valore è false, il rendering della sezione del calendario viene eseguito esattamente su EndDate, anche in presenza di uno spazio vuoto in una pagina. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | Ottiene o imposta un elenco di[`Gridline`](../../aspose.tasks.visualization/gridline/) che appaiono nella vista progetto. |
| [LegendOnEachPage](../../aspose.tasks.saving/saveoptions/legendoneachpage/) { get; set; } | Ottiene o imposta un valore che indica se la legenda deve essere visualizzata su ogni pagina (il valore predefinito è TRUE). |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | Ottiene o imposta un valore che indica se le attività critiche devono essere visualizzate in rosso (il valore predefinito è FALSE). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | Ottiene o imposta il colore dell'orario non lavorativo. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | Ottiene o imposta il numero di pagine del progetto. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | Ottiene o imposta le dimensioni della pagina di cui eseguire il rendering (il valore predefinito è PageSize.A4). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | Ottiene o imposta il[`PresentationFormat`](../saveoptions/presentationformat/) in cui verrà salvato il documento. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | Ottiene o imposta un valore che indica se il rendering di un progetto deve essere eseguito su una singola pagina quando il progetto viene salvato in formato grafico. La dimensione della pagina verrà modificata in modo che il progetto sottoposto a rendering possa essere contenuto in una pagina. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | Ottiene o imposta un valore che indica se le attività secondarie sulla barra delle attività di riepilogo devono essere contrassegnate. Per le attività secondarie, il campo Rollup indica se le informazioni sulle barre di Gantt delle attività secondarie verranno riportate nella barra delle attività di riepilogo. Per le attività di riepilogo, il Rollup Il campo indica se la barra delle attività di riepilogo visualizza le barre raggruppate. È necessario che il campo Riepilogo per le attività di riepilogo sia impostato su Sì affinché tutte le attività secondarie vengano raggruppate. |
| [SaveFormat](../../aspose.tasks.saving/saveoptions/saveformat/) { get; } | Ottiene o imposta il formato in cui verrà salvato il documento se viene utilizzato questo oggetto delle opzioni di salvataggio. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | Ottiene o imposta la data da cui iniziare il rendering. |
| [TasksComparer](../../aspose.tasks.saving/saveoptions/taskscomparer/) { get; set; } | Ottiene o imposta l'operatore di confronto per ordinare le attività nel diagramma di Gantt e nell'elenco delle attività. |
| [TasksFilter](../../aspose.tasks.saving/saveoptions/tasksfilter/) { get; set; } | Ottiene o imposta la condizione utilizzata per filtrare le attività visualizzate nei diagrammi Gantt, Foglio attività e Utilizzo attività. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | Ottiene o imposta l'elenco delle istanze di[`TextStyle`](../../aspose.tasks.visualization/textstyle/) classe che appare nella vista del progetto. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | Ottiene o imposta il[`Timescale`](../saveoptions/timescale/) valore utilizzato per controllare la modalità di rendering della scala cronologica (se presente) quando il progetto viene salvato in formato grafico. |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush/) { get; set; } | Ottiene o imposta un valore che indica se il pennello sfumatura deve essere utilizzato durante il rendering del diagramma di Gantt. |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | Ottiene o imposta un elenco delle colonne della vista di cui eseguire il rendering ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/) ). Se non impostato, vengono visualizzati solo ID attività, nomi attività, inizio e fine. Se sia Visualizza che[`ViewSettings`](../saveoptions/viewsettings/)le proprietà sono impostate, le colonne di View sovrascrivono le colonne di ViewSettings. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | Ottiene o imposta una vista ([`View`](../saveoptions/view/) ) rendere. Puoi utilizzare queste opzioni per specificare in modo esplicito quale vista deve essere salvata nei formati PDF, HTML o Immagine. Se questa proprietà è impostata,[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) proprietà viene ignorata quando il progetto viene salvato. La vista dovrebbe provenire da una delle seguenti schermate (([`Screen`](../../aspose.tasks/view/screen/) )): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |

### Guarda anche

* class [SaveOptions](../saveoptions/)
* spazio dei nomi [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assemblea [Aspose.Tasks](../../)


