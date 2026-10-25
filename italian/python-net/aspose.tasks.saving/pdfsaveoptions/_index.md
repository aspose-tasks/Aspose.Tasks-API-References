---
title: "PdfSaveOptions"
second_title: "Riferimento API di Aspose.Tasks per Python via .NET"
description: 
type: docs
weight: 90
url: /it/python-net/aspose.tasks.saving/pdfsaveoptions/
---

## PdfSaveOptions class

Consente di specificare opzioni aggiuntive durante il rendering delle pagine del progetto in PDF.

Il tipo PdfSaveOptions espone i seguenti membri:
## Costruttori
| Nome | Descrizione |
| :- | :- |
| PdfSaveOptions() | Inizializza una nuova istanza della classe [PdfSaveOptions](/tasks/python-net/aspose.tasks.saving/pdfsaveoptions/) che può essere utilizzata per salvare un documento in |
## Proprietà
| Nome | Descrizione |
| :- | :- |
| save_format |  |
| bar_styles | Ottiene o imposta l'elenco delle istanze della classe [BarStyle](/tasks/python-net/aspose.tasks.visualization/barstyle/) che compaiono nella visualizzazione del progetto. |
| draw_non_working_time | Ottiene o imposta un valore che indica se il tempo non lavorativo deve essere disegnato (Il valore predefinito è TRUE). |
| end_date | Ottiene o imposta una data fino a cui terminare il rendering. |
| timescale_fit_behavior | Ottiene o imposta un comportamento che definisce come allineare l'estremità destra della scala temporale con la fine della pagina. |
| fit_content | Ottiene o imposta un valore che indica se l'altezza della riga deve essere aumentata per adattarsi al contenuto. |
| gridlines | Ottiene o imposta un elenco di [Gridline](/tasks/python-net/aspose.tasks.visualization/gridline/) che appare nella visualizzazione del progetto. |
| legend_drawing_options | Ottiene o imposta un valore che definisce come renderizzare una legenda. Il valore predefinito è LegendDrawingOptions.OnEveryPage. |
| legend_items | Ottiene o imposta un array di PageLegendItem che definisce quali barre devono essere renderizzate nella legenda della pagina.<br/>            Se null, vengono renderizzati gli elementi predefiniti. |
| mark_critical_tasks | Ottiene o imposta un valore che indica se le attività critiche devono essere visualizzate in colore rosso (Il valore predefinito è FALSE). |
| non_working_time_color | Ottiene o imposta il colore del tempo non lavorativo. |
| page_count | Ottiene o imposta il numero di pagine del progetto. |
| page_size | Ottiene o imposta la dimensione della pagina da renderizzare (Il valore predefinito è PageSize.A4). |
| is_portrait | Ottiene o imposta un valore che indica se l'orientamento della pagina è verticale; restituisce false se l'orientamento della pagina è orizzontale. |
| presentation_format | Ottiene o imposta il [presentation_format](/tasks/python-net/aspose.tasks.saving/saveoptions/) in cui il documento verrà salvato. |
| roll_up_gantt_bars | Ottiene o imposta un valore che indica se le sottoattività sulla barra dell'attività di riepilogo devono essere contrassegnate.<br/>            Per le sottoattività, il campo Rollup indica se le informazioni sulle barre Gantt della sottoattività verranno aggregate nella barra dell'attività di riepilogo.<br/>            Per le attività di riepilogo, il campo Rollup indica se la barra dell'attività di riepilogo visualizza le barre aggregate.<br/>            È necessario impostare il campo Rollup per le attività di riepilogo su Yes affinché le sottoattività vengano aggregate. |
| start_date | Ottiene o imposta la data da cui iniziare il rendering. |
| text_styles | Ottiene o imposta l'elenco degli stili di testo applicati durante il rendering di una visualizzazione del progetto. |
| timescale | Ottiene o imposta il valore del [timescale](/tasks/python-net/aspose.tasks.saving/saveoptions/) che viene utilizzato per controllare come il timescale (se presente) viene renderizzato quando il progetto viene salvato in formato grafico. |
| use_gradient_brush | Ottiene o imposta un valore che indica se utilizzare un pennello gradiente durante il rendering del diagramma di Gantt. |
| view | Ottiene o imposta un elenco delle colonne della vista da renderizzare ([GanttChartColumn](/tasks/python-net/aspose.tasks.visualization/ganttchartcolumn/)).<br/>            Se non impostato, vengono renderizzati solo gli ID attività, i nomi delle attività, l'inizio e la fine.<br/>            Se sia la proprietà View sia le proprietà [view_settings](/tasks/python-net/aspose.tasks.saving/saveoptions/) sono impostate, le colonne da View sovrascrivono le colonne da ViewSettings. |
| view_settings | Ottiene o imposta una vista ([view](/tasks/python-net/aspose.tasks.saving/saveoptions/)) da renderizzare. È possibile utilizzare questa opzione per specificare esplicitamente quale vista deve essere salvata nei formati PDF, HTML o Image.<br/>            Se questa proprietà è impostata, la proprietà [PresentationFormat](/tasks/python-net/aspose.tasks.visualization/presentationformat/) viene ignorata quando il progetto viene salvato.<br/>            La vista deve provenire da una delle seguenti schermate (([screen](/tasks/python-net/aspose.tasks/view/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |
| custom_page_size | Ottiene o imposta la dimensione della pagina personalizzata in punti (1 punto = 1/72 di pollice). |
| render_to_single_page | Ottiene o imposta un valore che indica se un progetto deve essere renderizzato in una singola pagina<br/>            quando il progetto viene salvato in formato grafico.<br/>            La dimensione della pagina verrà modificata in modo che il progetto renderizzato possa stare su una pagina. |
| reduce_footer_gap | Ottiene o imposta un valore che indica se lo spazio tra l'ultima attività e il piè di pagina deve essere ridotto. |
| compliance | Ottiene o imposta il livello di conformità desiderato per il documento PDF generato.<br/>            Il valore predefinito è [PDF15](/tasks/python-net/aspose.tasks.saving/pdfcompliance/). |
| encryption_details | Ottiene o imposta i dettagli di crittografia. Se non impostato, non verrà eseguita alcuna crittografia. |
| text_compression | Ottiene o imposta un tipo di compressione da utilizzare per tutti i flussi di contenuto eccetto le immagini.<br/>            Il valore predefinito è [FLATE](/tasks/python-net/aspose.tasks.saving/pdftextcompression/). |
| digital_signature_details | Ottiene o imposta i dettagli della firma digitale. Se non impostato, non verrà eseguita alcuna firma. |
| save_to_separate_files | Ottiene o imposta un valore che indica se salvare le pagine del progetto in file separati. |
| page_saving_callback | Ottiene o imposta una callback definita dall'utente che viene utilizzata per ottenere uno stream di output per ogni pagina renderizzata.<br/>            È applicabile quando è usata l'opzione [save_to_separate_files](/tasks/python-net/aspose.tasks.saving/pdfsaveoptions/). |
| pages | Ottiene o imposta l'elenco dei numeri di pagina da salvare quando si salva il layout del progetto in file separati. |
| font_settings | Specifica le impostazioni dei font utilizzate durante il rendering della vista del progetto. |

### Vedi anche

* namespace [aspose.tasks.saving](/tasks/python-net/aspose.tasks.saving/)
* assembly [Aspose.Tasks](/tasks/python-net/)

