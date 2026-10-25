---
title: "Aspose::Tasks::Saving::SaveOptions class"
linktitle: "SaveOptions"
articleTitle: "SaveOptions"
second_title: "Aspose.Tasks per C++"
description: "Questa è una classe base astratta per le classi che consentono all'utente di specificare opzioni aggiuntive durante il salvataggio di un progetto in un formato particolare."
type: docs
weight: 10
url: /it/cpp/aspose.tasks.saving/saveoptions/
---

## SaveOptions class

**Inherits:** Aspose::Tasks::Saving::SimpleSaveOptions

Questa è una classe base astratta per le classi che consentono all'utente di specificare opzioni aggiuntive durante il salvataggio di un progetto in un formato particolare.

Un'istanza di qualsiasi classe derivata dalla classe SaveOptions viene passata alle overload di stream Save o string Save affinché l'utente possa definire opzioni personalizzate durante il salvataggio di un documento.

## Metodi

| Nome | Descrizione |
| --- | --- |
| [get_BarStyles](./get_barstyles/) | Restituisce l'elenco delle istanze della classe BarStyle che appaiono nella visualizzazione del progetto. |
| [get_CustomPageSize](./get_custompagesize/) | Restituisce la dimensione personalizzata della pagina in punti (1 punto = 1/72 di pollice). |
| [get_DrawNonWorkingTime](./get_drawnonworkingtime/) | Restituisce un valore che indica se il tempo non lavorativo deve essere disegnato (il valore predefinito è TRUE). |
| [get_EndDate](./get_enddate/) | Restituisce una data fino a cui terminare il rendering. |
| [get_FitContent](./get_fitcontent/) | Restituisce un valore che indica se l'altezza della riga deve essere aumentata per adattarsi al contenuto. |
| [get_FitTimescaleToEndOfPage](./get_fittimescaletoendofpage/) | Restituisce se una sezione calendario di una visualizzazione deve essere renderizzata fino alla fine (lato destro) dell'ultima pagina. Se il valore è false, la sezione calendario viene renderizzata esattamente fino a EndDate, anche se c'è uno spazio vuoto nella pagina. |
| [get_Gridlines](./get_gridlines/) | Restituisce un elenco di Gridline che appaiono nella visualizzazione del progetto. |
| [get_IsPortrait](./get_isportrait/) | Restituisce un valore che indica se l'orientamento della pagina è verticale; restituisce false se l'orientamento della pagina è orizzontale. |
| [get_LegendDrawingOptions](./get_legenddrawingoptions/) | Restituisce un valore che definisce come renderizzare una legenda. Il valore predefinito è LegendDrawingOptions.OnEveryPage. |
| [get_LegendItems](./get_legenditems/) | Restituisce un array di PageLegendItem che definiscono quali barre devono essere renderizzate nella legenda della pagina. Se null, vengono renderizzati gli elementi predefiniti. |
| [get_MarkCriticalTasks](./get_markcriticaltasks/) | Restituisce un valore che indica se le attività critiche devono essere visualizzate in colore rosso (il valore predefinito è FALSE). |
| [get_NonWorkingTimeColor](./get_nonworkingtimecolor/) | Restituisce il colore del tempo non lavorativo. |
| [get_PageCount](./get_pagecount/) | Restituisce il numero di pagine del progetto. |
| [get_PageSize](./get_pagesize/) | Restituisce la dimensione della pagina da renderizzare (il valore predefinito è PageSize.A4). |
| [get_PresentationFormat](./get_presentationformat/) | Restituisce il PresentationFormat in cui il documento sarà salvato. |
| [get_RenderToSinglePage](./get_rendertosinglepage/) | Restituisce un valore che indica se un progetto deve essere renderizzato su una singola pagina quando il progetto è salvato in formato grafico. La dimensione della pagina verrà modificata affinché il progetto renderizzato possa adattarsi a una pagina. |
| [get_RollUpGanttBars](./get_rollupganttbars/) | Restituisce un valore che indica se le sottoattività sulla barra dell'attività riepilogo devono essere contrassegnate. Per le sottoattività, il campo Rollup indica se le informazioni sulle barre Gantt della sottoattività verranno aggregate nella barra dell'attività riepilogo. Per le attività riepilogo, il campo Rollup indica se la barra dell'attività riepilogo visualizza le barre aggregate. È necessario impostare il campo Rollup per le attività riepilogo su Yes affinché le sottoattività vengano aggregate. |
| [get_StartDate](./get_startdate/) | Restituisce la data da cui iniziare il rendering. |
| [get_TextStyles](./get_textstyles/) | Restituisce l'elenco degli stili di testo applicati durante il rendering di una visualizzazione del progetto. |
| [get_Timescale](./get_timescale/) | Restituisce il valore Timescale utilizzato per controllare come la scala temporale (se presente) viene renderizzata quando il progetto è salvato in formato grafico. |
| [get_TimescaleFitBehavior](./get_timescalefitbehavior/) | Restituisce un comportamento che definisce come allineare l'estremità destra della scala temporale con il bordo della pagina. |
| [get_UseGradientBrush](./get_usegradientbrush/) | Restituisce un valore che indica se deve essere utilizzato un pennello a gradiente durante il rendering del diagramma di Gantt. |
| [get_View](./get_view/) | Ottiene un elenco delle colonne della vista da renderizzare ( GanttChartColumn ). Se non impostato, vengono renderizzati solo gli ID attività, i nomi delle attività, l'inizio e la fine. Se entrambe le proprietà View e ViewSettings sono impostate, le colonne da View sovrascrivono quelle da ViewSettings. |
| [get_ViewSettings](./get_viewsettings/) | Ottiene una vista ( View ) da renderizzare. È possibile utilizzare questa opzione per specificare esplicitamente quale vista deve essere salvata nei formati PDF, HTML o Immagine. Se questa proprietà è impostata, la proprietà Visualization::PresentationFormat viene ignorata quando il progetto viene salvato. La vista deve provenire da una delle seguenti schermate (( Aspose::Tasks::View::Screen )): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |
| [set_BarStyles](./set_barstyles/) | Imposta l'elenco delle istanze della classe BarStyle che appaiono nella vista del progetto. |
| [set_CustomPageSize](./set_custompagesize/) | Imposta la dimensione personalizzata della pagina in punti (1 punto = 1/72 di pollice). |
| [set_DrawNonWorkingTime](./set_drawnonworkingtime/) | Imposta un valore che indica se il tempo non lavorativo deve essere disegnato (Il valore predefinito è TRUE). |
| [set_EndDate](./set_enddate/) | Imposta una data per terminare il rendering. |
| [set_FitContent](./set_fitcontent/) | Imposta un valore che indica se l'altezza della riga deve essere aumentata per adattarsi al contenuto. |
| [set_FitTimescaleToEndOfPage](./set_fittimescaletoendofpage/) | Imposta se una sezione calendario di una vista deve essere renderizzata fino alla fine (lato destro) dell'ultima pagina. Se il valore è false, la sezione calendario viene renderizzata esattamente fino a EndDate, anche se c'è uno spazio vuoto nella pagina. |
| [set_Gridlines](./set_gridlines/) | Imposta un elenco di Gridline che appare nella vista del progetto. |
| [set_IsPortrait](./set_isportrait/) | Imposta un valore che indica se l'orientamento della pagina è verticale; restituisce false se l'orientamento della pagina è orizzontale. |
| [set_LegendDrawingOptions](./set_legenddrawingoptions/) | Imposta un valore che definisce come renderizzare una legenda. Il valore predefinito è LegendDrawingOptions.OnEveryPage. |
| [set_LegendItems](./set_legenditems/) | Imposta un array di PageLegendItem che definisce quali barre devono essere renderizzate nella legenda della pagina. Se null, vengono renderizzati gli elementi predefiniti. |
| [set_MarkCriticalTasks](./set_markcriticaltasks/) | Imposta un valore che indica se le attività critiche devono essere visualizzate in colore rosso (Il valore predefinito è FALSE). |
| [set_NonWorkingTimeColor](./set_nonworkingtimecolor/) | Imposta il colore del tempo non lavorativo. |
| [set_PageSize](./set_pagesize/) | Imposta la dimensione della pagina da renderizzare (Il valore predefinito è PageSize.A4). |
| [set_PresentationFormat](./set_presentationformat/) | Imposta il PresentationFormat in cui il documento sarà salvato. |
| [set_RenderToSinglePage](./set_rendertosinglepage/) | Imposta un valore che indica se un progetto deve essere renderizzato su una singola pagina quando il progetto è salvato in formato grafico. La dimensione della pagina verrà modificata in modo che il progetto renderizzato possa adattarsi a una pagina. |
| [set_RollUpGanttBars](./set_rollupganttbars/) | Imposta un valore che indica se le sottoattività sulla barra dell'attività riepilogo devono essere contrassegnate. Per le sottoattività, il campo Rollup indica se le informazioni sulle barre Gantt della sottoattività verranno aggregate nella barra dell'attività riepilogo. Per le attività riepilogo, il campo Rollup indica se la barra dell'attività riepilogo visualizza le barre aggregate. È necessario impostare il campo Rollup per le attività riepilogo su Yes affinché le sottoattività vengano aggregate. |
| [set_StartDate](./set_startdate/) | Imposta la data da cui iniziare il rendering. |
| [set_TextStyles](./set_textstyles/) | Imposta l'elenco degli stili di testo applicati durante il rendering di una vista del progetto. |
| [set_Timescale](./set_timescale/) | Imposta il valore Timescale utilizzato per controllare come la scala temporale (se presente) viene renderizzata quando il progetto è salvato in formato grafico. |
| [set_TimescaleFitBehavior](./set_timescalefitbehavior/) | Imposta un comportamento che definisce come allineare l'estremità destra della scala temporale con la fine della pagina. |
| [set_UseGradientBrush](./set_usegradientbrush/) | Imposta un valore che indica se deve essere utilizzato un pennello gradiente durante il rendering del Gantt Chart. |
| [set_View](./set_view/) | Imposta un elenco delle colonne della vista da renderizzare ( GanttChartColumn ). Se non impostato, vengono renderizzati solo gli ID attività, i nomi delle attività, l'inizio e la fine. Se entrambe le proprietà View e ViewSettings sono impostate, le colonne da View sovrascrivono quelle da ViewSettings. |
| [set_ViewSettings](./set_viewsettings/) | Imposta una vista ( View ) da renderizzare. È possibile utilizzare questa opzione per specificare esplicitamente quale vista deve essere salvata nei formati PDF, HTML o Immagine. Se questa proprietà è impostata, la proprietà Visualization::PresentationFormat viene ignorata quando il progetto viene salvato. La vista deve provenire da una delle seguenti schermate (( Aspose::Tasks::View::Screen )): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |

