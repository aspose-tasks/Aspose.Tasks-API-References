---
title: "SaveOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "Questa è una classe base astratta per classi che consentono all'utente di specificare opzioni aggiuntive durante il salvataggio di un progetto in un formato specifico."
type: docs
weight: 274
url: /it/java/com.aspose.tasks/saveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public abstract class SaveOptions extends SimpleSaveOptions
```

Questa è una classe base astratta per classi che consentono all'utente di specificare opzioni aggiuntive durante il salvataggio di un progetto in un formato specifico.

--------------------

Un'istanza di qualsiasi classe derivata dalla classe SaveOptions viene passata ai sovraccarichi di Save su stream o su stringa affinché l'utente possa definire opzioni personalizzate durante il salvataggio di un documento.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getBarStyles()](#getBarStyles--) | Restituisce l'elenco delle istanze della classe [BarStyle](../../com.aspose.tasks/barstyle) che appaiono nella vista del progetto. |
| [getCustomPageSize()](#getCustomPageSize--) | Restituisce la dimensione personalizzata della pagina in punti (1 punto = 1/72 di pollice). |
| [getDrawNonWorkingTime()](#getDrawNonWorkingTime--) | Restituisce un valore che indica se il tempo non lavorativo deve essere disegnato (il valore predefinito è TRUE). |
| [getEndDate()](#getEndDate--) | Restituisce una data fino a cui terminare il rendering. |
| [getFitContent()](#getFitContent--) | Restituisce un valore che indica se l'altezza della riga deve essere aumentata per adattarsi al contenuto. |
| [getGridlines()](#getGridlines--) | Restituisce un elenco di [Gridline](../../com.aspose.tasks/gridline) che appaiono nella vista del progetto. |
| [getLegendDrawingOptions()](#getLegendDrawingOptions--) | Restituisce un valore che definisce come renderizzare una legenda. |
| [getLegendItems()](#getLegendItems--) | Restituisce un array di PageLegendItem che definisce quali barre devono essere renderizzate nella legenda della pagina. |
| [getMarkCriticalTasks()](#getMarkCriticalTasks--) | Restituisce un valore che indica se le attività critiche devono essere visualizzate in colore rosso (il valore predefinito è FALSE). |
| [getNonWorkingTimeColor()](#getNonWorkingTimeColor--) | Restituisce il colore del tempo non lavorativo. |
| [getPageCount()](#getPageCount--) | Restituisce il numero di pagine del progetto. |
| [getPageSize()](#getPageSize--) | Restituisce la dimensione della pagina da renderizzare (il valore predefinito è PageSize.A4). |
| [getPresentationFormat()](#getPresentationFormat--) | Ottiene il `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) in cui il documento verrà salvato. |
| [getRenderToSinglePage()](#getRenderToSinglePage--) | Ottiene un valore che indica se un progetto deve essere renderizzato in una singola pagina quando il progetto viene salvato in formato grafico. |
| [getRollUpGanttBars()](#getRollUpGanttBars--) | Ottiene un valore che indica se le sottoattività sulla barra dell'attività di riepilogo devono essere contrassegnate. |
| [getStartDate()](#getStartDate--) | Ottiene la data da cui iniziare il rendering. |
| [getTaskLinkDrawingCallback()](#getTaskLinkDrawingCallback--) | Ottiene una callback che può essere utilizzata per personalizzare alcuni aspetti del rendering dei collegamenti delle attività. |
| [getTextStyles()](#getTextStyles--) | Ottiene l'elenco degli stili di testo applicati durante il rendering di una vista di progetto. |
| [getTimescale()](#getTimescale--) | Ottiene il valore `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) che viene usato per controllare come la scala temporale (se presente) viene renderizzata quando il progetto è salvato in formato grafico. |
| [getTimescaleFitBehavior()](#getTimescaleFitBehavior--) | Ottiene un comportamento che definisce come allineare l'estremità destra della scala temporale con la fine della pagina. |
| [getUseGradientBrush()](#getUseGradientBrush--) | Ottiene un valore che indica se deve essere usato un pennello a gradiente durante il rendering del diagramma di Gantt. |
| [getView()](#getView--) | Ottiene un elenco delle colonne della vista da renderizzare ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |
| [getViewSettings()](#getViewSettings--) | Ottiene una vista (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) da renderizzare. |
| [isPortrait()](#isPortrait--) | Restituisce un valore che indica se l'orientamento della pagina è verticale; restituisce false se l'orientamento della pagina è orizzontale. |
| [setBarStyles(List&lt;BarStyle&gt; value)](#setBarStyles-java.util.List-com.aspose.tasks.BarStyle--) | Imposta l'elenco delle istanze della classe [BarStyle](../../com.aspose.tasks/barstyle) che appaiono nella vista di progetto. |
| [setCustomPageSize(Dimension2D value)](#setCustomPageSize-java.awt.geom.Dimension2D-) | Imposta la dimensione personalizzata della pagina in punti (1 punto = 1/72 di pollice). |
| [setDrawNonWorkingTime(boolean value)](#setDrawNonWorkingTime-boolean-) | Imposta un valore che indica se il tempo non lavorativo deve essere disegnato (Il valore predefinito è TRUE). |
| [setEndDate(Date value)](#setEndDate-java.util.Date-) | Imposta una data fino a cui terminare il rendering. |
| [setFitContent(boolean value)](#setFitContent-boolean-) | Imposta un valore che indica se l'altezza della riga deve essere aumentata per adattarsi al contenuto. |
| [setGridlines(List&lt;Gridline&gt; value)](#setGridlines-java.util.List-com.aspose.tasks.Gridline--) | Imposta un elenco di [Gridline](../../com.aspose.tasks/gridline) che appaiono nella vista di progetto. |
| [setLegendDrawingOptions(int value)](#setLegendDrawingOptions-int-) | Imposta un valore che definisce come renderizzare una legenda. |
| [setLegendItems(PageLegendItem[] value)](#setLegendItems-com.aspose.tasks.PageLegendItem---) | Imposta un array di PageLegendItem che definisce quali barre devono essere renderizzate nella legenda della pagina. |
| [setMarkCriticalTasks(boolean value)](#setMarkCriticalTasks-boolean-) | Imposta un valore che indica se le attività critiche devono essere visualizzate in colore rosso (Il valore predefinito è FALSE). |
| [setNonWorkingTimeColor(Color value)](#setNonWorkingTimeColor-java.awt.Color-) | Imposta il colore del tempo non lavorativo. |
| [setPageSize(int value)](#setPageSize-int-) | Imposta la dimensione della pagina da renderizzare (Il valore predefinito è PageSize.A4). |
| [setPortrait(boolean value)](#setPortrait-boolean-) | Imposta un valore che indica se l'orientamento della pagina è verticale; restituisce false se l'orientamento della pagina è orizzontale. |
| [setPresentationFormat(int value)](#setPresentationFormat-int-) | Imposta il `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) in cui il documento verrà salvato. |
| [setRenderToSinglePage(boolean value)](#setRenderToSinglePage-boolean-) | Imposta un valore che indica se un progetto deve essere renderizzato in una singola pagina quando il progetto è salvato in formato grafico. |
| [setRollUpGanttBars(boolean value)](#setRollUpGanttBars-boolean-) | Imposta un valore che indica se le sottoattività sulla barra dell'attività di riepilogo devono essere contrassegnate. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Imposta la data da cui iniziare il rendering. |
| [setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value)](#setTaskLinkDrawingCallback-com.aspose.tasks.TaskLinkDrawingCallbackDelegate-) | Imposta una callback che può essere usata per personalizzare alcuni aspetti del rendering dei collegamenti delle attività. |
| [setTextStyles(List&lt;TextStyle&gt; value)](#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--) | Imposta l'elenco degli stili di testo applicati durante il rendering di una vista di progetto. |
| [setTimescale(int value)](#setTimescale-int-) | Imposta il valore `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) che è usato per controllare come la scala temporale (se presente) viene renderizzata quando il progetto è salvato in formato grafico. |
| [setTimescaleFitBehavior(int value)](#setTimescaleFitBehavior-int-) | Imposta un comportamento che definisce come allineare l'estremità destra della scala temporale con il bordo della pagina. |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | Imposta un valore che indica se deve essere usato un pennello gradiente durante il rendering del diagramma di Gantt. |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | Imposta un elenco delle colonne della vista da renderizzare ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |
| [setViewSettings(View value)](#setViewSettings-com.aspose.tasks.View-) | Imposta una vista (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) da renderizzare. |
### getBarStyles() {#getBarStyles--}
```
public final List<BarStyle> getBarStyles()
```


Restituisce l'elenco delle istanze della classe [BarStyle](../../com.aspose.tasks/barstyle) che appaiono nella vista del progetto.

**Returns:**
java.util.List&lt;com.aspose.tasks.BarStyle&gt; - l'elenco delle istanze della classe [BarStyle](../../com.aspose.tasks/barstyle) che appaiono nella vista del progetto.
### getCustomPageSize() {#getCustomPageSize--}
```
public final Dimension2D getCustomPageSize()
```


Restituisce la dimensione personalizzata della pagina in punti (1 punto = 1/72 di pollice).

**Returns:**
java.awt.geom.Dimension2D - la dimensione personalizzata della pagina in punti (1 punto = 1/72 di pollice).
### getDrawNonWorkingTime() {#getDrawNonWorkingTime--}
```
public final boolean getDrawNonWorkingTime()
```


Restituisce un valore che indica se il tempo non lavorativo deve essere disegnato (il valore predefinito è TRUE).

**Returns:**
boolean - un valore che indica se il tempo non lavorativo deve essere disegnato (Il valore predefinito è TRUE).
### getEndDate() {#getEndDate--}
```
public final Date getEndDate()
```


Restituisce una data fino a cui terminare il rendering.

**Returns:**
java.util.Date - una data fino a cui terminare il rendering.
### getFitContent() {#getFitContent--}
```
public final boolean getFitContent()
```


Restituisce un valore che indica se l'altezza della riga deve essere aumentata per adattarsi al contenuto.

**Returns:**
boolean - un valore che indica se l'altezza della riga deve essere aumentata per adattarsi al contenuto.
### getGridlines() {#getGridlines--}
```
public final List<Gridline> getGridlines()
```


Restituisce un elenco di [Gridline](../../com.aspose.tasks/gridline) che appaiono nella vista del progetto.

**Returns:**
java.util.List&lt;com.aspose.tasks.Gridline&gt; - un elenco di [Gridline](../../com.aspose.tasks/gridline) che appaiono nella vista del progetto.
### getLegendDrawingOptions() {#getLegendDrawingOptions--}
```
public final int getLegendDrawingOptions()
```


Ottiene un valore che definisce come renderizzare una legenda. Il valore predefinito è LegendDrawingOptions.OnEveryPage.

È applicabile solo quando la vista del diagramma di Gantt è renderizzata.

**Returns:**
int - un valore che definisce come renderizzare una legenda.
### getLegendItems() {#getLegendItems--}
```
public final PageLegendItem[] getLegendItems()
```


Ottiene un array di PageLegendItem che definisce quali barre devono essere renderizzate nella legenda della pagina. Se null, vengono renderizzati gli elementi predefiniti.

È applicabile solo quando la vista del diagramma di Gantt è renderizzata.

**Returns:**
com.aspose.tasks.PageLegendItem[] - un array di PageLegendItem che definisce quali barre devono essere renderizzate nella legenda della pagina.
### getMarkCriticalTasks() {#getMarkCriticalTasks--}
```
public final boolean getMarkCriticalTasks()
```


Restituisce un valore che indica se le attività critiche devono essere visualizzate in colore rosso (il valore predefinito è FALSE).

**Returns:**
boolean - un valore che indica se le attività critiche devono essere visualizzate in colore rosso (Il valore predefinito è FALSE).
### getNonWorkingTimeColor() {#getNonWorkingTimeColor--}
```
public final Color getNonWorkingTimeColor()
```


Restituisce il colore del tempo non lavorativo.

**Returns:**
java.awt.Color - il colore del tempo non lavorativo.
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Restituisce il numero di pagine del progetto.

**Returns:**
int - il numero di pagine del progetto.
### getPageSize() {#getPageSize--}
```
public final int getPageSize()
```


Restituisce la dimensione della pagina da renderizzare (il valore predefinito è PageSize.A4).

**Returns:**
int - la dimensione della pagina da renderizzare (Il valore predefinito è PageSize.A4).
### getPresentationFormat() {#getPresentationFormat--}
```
public final int getPresentationFormat()
```


Ottiene il `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) in cui il documento verrà salvato.

**Returns:**
int - il `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) in cui il documento sarà salvato.
### getRenderToSinglePage() {#getRenderToSinglePage--}
```
public final boolean getRenderToSinglePage()
```


Ottiene un valore che indica se un progetto deve essere renderizzato su una singola pagina quando il progetto è salvato in formato grafico. La dimensione della pagina sarà modificata in modo che il progetto renderizzato possa adattarsi a una pagina.

**Returns:**
boolean - un valore che indica se un progetto deve essere renderizzato in una singola pagina quando il progetto è salvato in formato grafico.
### getRollUpGanttBars() {#getRollUpGanttBars--}
```
public final boolean getRollUpGanttBars()
```


Restituisce un valore che indica se le sottoattività sulla barra dell'attività riepilogo devono essere contrassegnate. Per le sottoattività, il campo Rollup indica se le informazioni sulle barre Gantt della sottoattività verranno aggregate nella barra dell'attività riepilogo. Per le attività riepilogo, il campo Rollup indica se la barra dell'attività riepilogo visualizza barre aggregate. È necessario impostare il campo Rollup per le attività riepilogo su Sì affinché le sottoattività vengano aggregate.

--------------------

È applicabile solo quando la vista del diagramma di Gantt è renderizzata.

**Returns:**
boolean - un valore che indica se le sottoattività sulla barra dell'attività riepilogo devono essere contrassegnate.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


Ottiene la data da cui iniziare il rendering.

**Returns:**
java.util.Date - la data da cui iniziare il rendering.
### getTaskLinkDrawingCallback() {#getTaskLinkDrawingCallback--}
```
public final TaskLinkDrawingCallbackDelegate getTaskLinkDrawingCallback()
```


Ottiene una callback che può essere utilizzata per personalizzare alcuni aspetti del rendering dei collegamenti delle attività.

È applicabile solo quando la vista del diagramma di Gantt è renderizzata.

**Returns:**
[TaskLinkDrawingCallbackDelegate](../../com.aspose.tasks/tasklinkdrawingcallbackdelegate) - a callback that can be used to customize some aspects of task links rendering.
### getTextStyles() {#getTextStyles--}
```
public final List<TextStyle> getTextStyles()
```


Ottiene l'elenco degli stili di testo applicati durante il rendering di una vista di progetto.

--------------------

Questi stili sovrascrivono gli stili definiti con GanttCharView.setTextStyles.

**Returns:**
java.util.List&lt;com.aspose.tasks.TextStyle&gt; - l'elenco degli stili di testo applicati durante il rendering di una vista di progetto.
### getTimescale() {#getTimescale--}
```
public final int getTimescale()
```


Ottiene il valore `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) che viene usato per controllare come la scala temporale (se presente) viene renderizzata quando il progetto è salvato in formato grafico.

**Returns:**
int - il valore `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) utilizzato per controllare come la scala temporale (se presente) viene renderizzata quando il progetto è salvato in formato grafico.
### getTimescaleFitBehavior() {#getTimescaleFitBehavior--}
```
public final int getTimescaleFitBehavior()
```


Ottiene un comportamento che definisce come allineare l'estremità destra della scala temporale con la fine della pagina.

**Returns:**
int - un comportamento che definisce come allineare l'estremità destra della scala temporale con il margine della pagina.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


Ottiene un valore che indica se deve essere usato un pennello a gradiente durante il rendering del diagramma di Gantt.

--------------------

È applicabile solo quando la vista del diagramma di Gantt è renderizzata.

**Returns:**
boolean - un valore che indica se deve essere utilizzato un pennello gradiente durante il rendering del diagramma di Gantt.
### getView() {#getView--}
```
public final ProjectView getView()
```


Restituisce un elenco delle colonne della vista da renderizzare ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). Se non impostato, vengono renderizzati solo gli ID attività, i nomi delle attività, l'inizio e la fine. Se entrambe le proprietà View e `ViewSettings`([getViewSettings()](../../com.aspose.tasks/saveoptions\#getViewSettings--)/[setViewSettings(View)](../../com.aspose.tasks/saveoptions\#setViewSettings-View-)) sono impostate, le colonne della View sovrascrivono quelle di ViewSettings.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns to render ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)).
### getViewSettings() {#getViewSettings--}
```
public final View getViewSettings()
```


Restituisce una vista (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) da renderizzare. È possibile utilizzare questa opzione per specificare esplicitamente quale vista deve essere salvata nei formati PDF, HTML o Image. Se questa proprietà è impostata, la proprietà [PresentationFormat](../../com.aspose.tasks/presentationformat) viene ignorata quando il progetto è salvato. La vista deve provenire da una delle seguenti schermate ((`Aspose.Tasks.View.Screen`([View.getScreen()](../../com.aspose.tasks/view\#getScreen--)/[View.setScreen(int)](../../com.aspose.tasks/view\#setScreen-int-)))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage)

**Returns:**
[View](../../com.aspose.tasks/view) - a view (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) to render.
### isPortrait() {#isPortrait--}
```
public final boolean isPortrait()
```


Restituisce un valore che indica se l'orientamento della pagina è verticale; restituisce false se l'orientamento della pagina è orizzontale.

--------------------

Non è applicabile quando SaveOptions.getPageSize() == PageSize.DefinedInView. In questo caso viene utilizzato [PageSettings.isPortrait()](../../com.aspose.tasks/pagesettings\#isPortrait--). Non è applicabile quando è impostato [getCustomPageSize()](../../com.aspose.tasks/saveoptions\#getCustomPageSize--).

**Returns:**
boolean - un valore che indica se l'orientamento della pagina è verticale; restituisce false se l'orientamento della pagina è orizzontale.
### setBarStyles(List&lt;BarStyle&gt; value) {#setBarStyles-java.util.List-com.aspose.tasks.BarStyle--}
```
public final void setBarStyles(List<BarStyle> value)
```


Imposta l'elenco delle istanze della classe [BarStyle](../../com.aspose.tasks/barstyle) che appaiono nella vista di progetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.BarStyle&gt; | l'elenco delle istanze della classe [BarStyle](../../com.aspose.tasks/barstyle) che compaiono nella vista del progetto. |

### setCustomPageSize(Dimension2D value) {#setCustomPageSize-java.awt.geom.Dimension2D-}
```
public final void setCustomPageSize(Dimension2D value)
```


Imposta la dimensione personalizzata della pagina in punti (1 punto = 1/72 di pollice).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.awt.geom.Dimension2D | la dimensione personalizzata della pagina in punti (1 punto = 1/72 di pollice). |

### setDrawNonWorkingTime(boolean value) {#setDrawNonWorkingTime-boolean-}
```
public final void setDrawNonWorkingTime(boolean value)
```


Imposta un valore che indica se il tempo non lavorativo deve essere disegnato (Il valore predefinito è TRUE).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se il tempo non lavorativo deve essere disegnato (Il valore predefinito è TRUE). |

### setEndDate(Date value) {#setEndDate-java.util.Date-}
```
public final void setEndDate(Date value)
```


Imposta una data fino a cui terminare il rendering.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date | una data fino a cui terminare il rendering. |

### setFitContent(boolean value) {#setFitContent-boolean-}
```
public final void setFitContent(boolean value)
```


Imposta un valore che indica se l'altezza della riga deve essere aumentata per adattarsi al contenuto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se l'altezza della riga deve essere aumentata per adattarsi al contenuto. |

### setGridlines(List&lt;Gridline&gt; value) {#setGridlines-java.util.List-com.aspose.tasks.Gridline--}
```
public final void setGridlines(List<Gridline> value)
```


Imposta un elenco di [Gridline](../../com.aspose.tasks/gridline) che appaiono nella vista di progetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.Gridline&gt; | un elenco di [Gridline](../../com.aspose.tasks/gridline) che compaiono nella vista del progetto. |

### setLegendDrawingOptions(int value) {#setLegendDrawingOptions-int-}
```
public final void setLegendDrawingOptions(int value)
```


Imposta un valore che definisce come renderizzare una legenda. Il valore predefinito è LegendDrawingOptions.OnEveryPage.

È applicabile solo quando la vista del diagramma di Gantt è renderizzata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | un valore che definisce come renderizzare una legenda. |

### setLegendItems(PageLegendItem[] value) {#setLegendItems-com.aspose.tasks.PageLegendItem---}
```
public final void setLegendItems(PageLegendItem[] value)
```


Imposta un array di PageLegendItem che definisce quali barre devono essere renderizzate nella legenda della pagina. Se null, vengono renderizzati gli elementi predefiniti.

È applicabile solo quando la vista del diagramma di Gantt è renderizzata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [PageLegendItem\[\]](../../com.aspose.tasks/pagelegenditem) | un array di PageLegendItem che definisce quali barre devono essere renderizzate nella legenda della pagina. |

### setMarkCriticalTasks(boolean value) {#setMarkCriticalTasks-boolean-}
```
public final void setMarkCriticalTasks(boolean value)
```


Imposta un valore che indica se le attività critiche devono essere visualizzate in colore rosso (Il valore predefinito è FALSE).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se le attività critiche devono essere visualizzate in colore rosso (Il valore predefinito è FALSE). |

### setNonWorkingTimeColor(Color value) {#setNonWorkingTimeColor-java.awt.Color-}
```
public final void setNonWorkingTimeColor(Color value)
```


Imposta il colore del tempo non lavorativo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.awt.Color | il colore del tempo non lavorativo. |

### setPageSize(int value) {#setPageSize-int-}
```
public final void setPageSize(int value)
```


Imposta la dimensione della pagina da renderizzare (Il valore predefinito è PageSize.A4).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | la dimensione della pagina da renderizzare (Il valore predefinito è PageSize.A4). |

### setPortrait(boolean value) {#setPortrait-boolean-}
```
public final void setPortrait(boolean value)
```


Imposta un valore che indica se l'orientamento della pagina è verticale; restituisce false se l'orientamento della pagina è orizzontale.

--------------------

Non è applicabile quando SaveOptions.PageSize == Visualization.PageSize.DefinedInView. In questo caso [PageSettings.setPortrait(boolean)](../../com.aspose/tasks/pagesettings\#setPortrait-boolean-) è usato al suo posto. Non è applicabile quando [getCustomPageSize()](../../com.aspose.tasks/saveoptions\#getCustomPageSize--) è impostato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se l'orientamento della pagina è verticale; restituisce false se l'orientamento della pagina è orizzontale. |

### setPresentationFormat(int value) {#setPresentationFormat-int-}
```
public final void setPresentationFormat(int value)
```


Imposta il `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) in cui il documento verrà salvato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | int | il `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) in cui il documento verrà salvato. |

### setRenderToSinglePage(boolean value) {#setRenderToSinglePage-boolean-}
```
public final void setRenderToSinglePage(boolean value)
```


Imposta un valore che indica se un progetto deve essere renderizzato su una singola pagina quando il progetto è salvato in formato grafico. La dimensione della pagina verrà modificata in modo che il progetto renderizzato possa adattarsi a una pagina.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se un progetto deve essere renderizzato su una singola pagina quando il progetto è salvato in formato grafico. |

### setRollUpGanttBars(boolean value) {#setRollUpGanttBars-boolean-}
```
public final void setRollUpGanttBars(boolean value)
```


Imposta un valore che indica se le sottoattività sulla barra dell'attività di riepilogo devono essere contrassegnate. Per le sottoattività, il campo Rollup indica se le informazioni sulle barre Gantt della sottoattività saranno aggregate nella barra dell'attività di riepilogo. Per le attività di riepilogo, il campo Rollup indica se la barra dell'attività di riepilogo visualizza barre aggregate. È necessario impostare il campo Rollup per le attività di riepilogo su Sì affinché le sottoattività vengano aggregate.

--------------------

È applicabile solo quando la vista del diagramma di Gantt è renderizzata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se le sottoattività sulla barra dell'attività di riepilogo devono essere contrassegnate. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


Imposta la data da cui iniziare il rendering.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date | la data da cui iniziare il rendering. |

### setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value) {#setTaskLinkDrawingCallback-com.aspose.tasks.TaskLinkDrawingCallbackDelegate-}
```
public final void setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value)
```


Imposta una callback che può essere usata per personalizzare alcuni aspetti del rendering dei collegamenti delle attività.

È applicabile solo quando la vista del diagramma di Gantt è renderizzata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [TaskLinkDrawingCallbackDelegate](../../com.aspose.tasks/tasklinkdrawingcallbackdelegate) | una callback che può essere usata per personalizzare alcuni aspetti del rendering dei collegamenti delle attività. |

### setTextStyles(List&lt;TextStyle&gt; value) {#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--}
```
public final void setTextStyles(List<TextStyle> value)
```


Imposta l'elenco degli stili di testo applicati durante il rendering di una vista di progetto.

--------------------

Questi stili sovrascrivono gli stili definiti con GanttCharView.setTextStyles.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.List&lt;com.aspose.tasks.TextStyle&gt; | l'elenco degli stili di testo applicati durante il rendering di una vista di progetto. |

### setTimescale(int value) {#setTimescale-int-}
```
public final void setTimescale(int value)
```


Imposta il valore `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) che è usato per controllare come la scala temporale (se presente) viene renderizzata quando il progetto è salvato in formato grafico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | int | il valore `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) che viene usato per controllare come la scala temporale (se presente) viene renderizzata quando il progetto è salvato in formato grafico. |

### setTimescaleFitBehavior(int value) {#setTimescaleFitBehavior-int-}
```
public final void setTimescaleFitBehavior(int value)
```


Imposta un comportamento che definisce come allineare l'estremità destra della scala temporale con il bordo della pagina.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | un comportamento che definisce come allineare l'estremità destra della scala temporale con il bordo della pagina. |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


Imposta un valore che indica se deve essere usato un pennello gradiente durante il rendering del diagramma di Gantt.

--------------------

È applicabile solo quando la vista del diagramma di Gantt è renderizzata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se deve essere usato un pennello gradiente durante il rendering del diagramma di Gantt. |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


Imposta un elenco delle colonne della vista da renderizzare ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). Se non impostato, vengono renderizzati solo gli ID delle attività, i nomi delle attività, l'inizio e la fine. Se sia View sia le proprietà `ViewSettings`([getViewSettings()](../../com.aspose.tasks/saveoptions\#getViewSettings--)/[setViewSettings(View)](../../com.aspose.tasks/saveoptions\#setViewSettings-View-)) sono impostate, le colonne da View sovrascrivono le colonne da ViewSettings.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | un elenco delle colonne della vista da renderizzare ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |

### setViewSettings(View value) {#setViewSettings-com.aspose.tasks.View-}
```
public final void setViewSettings(View value)
```


Imposta una vista (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) da renderizzare. È possibile utilizzare questa opzione per specificare esplicitamente quale vista deve essere salvata nei formati PDF, HTML o Image. Se questa proprietà è impostata, la proprietà [PresentationFormat](../../com.aspose.tasks/presentationformat) viene ignorata quando il progetto è salvato. La vista deve provenire da una delle seguenti schermate ((`Aspose.Tasks.View.Screen`([View.getScreen()](../../com.aspose.tasks/view\#getScreen--)/[View.setScreen(int)](../../com.aspose.tasks/view\#setScreen-int-)))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage)

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [View](../../com.aspose.tasks/view) | una vista (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) da renderizzare. |

