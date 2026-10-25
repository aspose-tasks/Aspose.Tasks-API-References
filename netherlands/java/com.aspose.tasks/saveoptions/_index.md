---
title: "SaveOptions"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Dit is een abstracte basisklasse voor klassen die de gebruiker in staat stellen extra opties op te geven bij het opslaan van een project in een bepaald formaat."
type: docs
weight: 274
url: /nl/java/com.aspose.tasks/saveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public abstract class SaveOptions extends SimpleSaveOptions
```

Dit is een abstracte basisklasse voor klassen die de gebruiker in staat stellen extra opties op te geven bij het opslaan van een project in een bepaald formaat.

--------------------

Een exemplaar van elke afgeleide klasse van de SaveOptions-klasse wordt doorgegeven aan de stream Save- of string Save-overloads zodat de gebruiker aangepaste opties kan definiëren bij het opslaan van een document.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getBarStyles()](#getBarStyles--) | Haalt de lijst op van de exemplaren van de [BarStyle](../../com.aspose/tasks/barstyle) klasse die verschijnen in de projectweergave. |
| [getCustomPageSize()](#getCustomPageSize--) | Haalt de aangepaste paginagrootte op in points (1 point = 1/72 inch). |
| [getDrawNonWorkingTime()](#getDrawNonWorkingTime--) | Haalt een waarde op die aangeeft of niet-werkelijke tijd moet worden getekend (standaardwaarde is TRUE). |
| [getEndDate()](#getEndDate--) | Haalt een datum op waarop het renderen moet worden beëindigd. |
| [getFitContent()](#getFitContent--) | Haalt een waarde op die aangeeft of de rijhoogte moet worden vergroot om de inhoud te passen. |
| [getGridlines()](#getGridlines--) | Haalt een lijst op van [Gridline](../../com.aspose/tasks/gridline) die verschijnen in de projectweergave. |
| [getLegendDrawingOptions()](#getLegendDrawingOptions--) | Haalt een waarde op die bepaalt hoe een legenda moet worden gerenderd. |
| [getLegendItems()](#getLegendItems--) | Haalt een array op van PageLegendItem die bepalen welke balken in de paginalegenda moeten worden gerenderd. |
| [getMarkCriticalTasks()](#getMarkCriticalTasks--) | Haalt een waarde op die aangeeft of kritieke taken in rode kleur moeten worden weergegeven (standaardwaarde is FALSE). |
| [getNonWorkingTimeColor()](#getNonWorkingTimeColor--) | Haalt de kleur van niet-werkelijke tijd op. |
| [getPageCount()](#getPageCount--) | Haalt het aantal pagina's van het project op. |
| [getPageSize()](#getPageSize--) | Haalt de grootte van de te renderen pagina op (standaardwaarde is PageSize.A4). |
| [getPresentationFormat()](#getPresentationFormat--) | Haalt het `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) op waarin het document wordt opgeslagen. |
| [getRenderToSinglePage()](#getRenderToSinglePage--) | Haalt een waarde op die aangeeft of een project moet worden gerenderd op één pagina wanneer het project wordt opgeslagen in een grafisch formaat. |
| [getRollUpGanttBars()](#getRollUpGanttBars--) | Haalt een waarde op die aangeeft of subtaken op de samenvattingsbalk gemarkeerd moeten worden. |
| [getStartDate()](#getStartDate--) | Haalt de datum op vanaf wanneer gerenderd moet worden. |
| [getTaskLinkDrawingCallback()](#getTaskLinkDrawingCallback--) | Haalt een callback op die kan worden gebruikt om enkele aspecten van het renderen van taaklinks aan te passen. |
| [getTextStyles()](#getTextStyles--) | Haalt de lijst met tekststijlen op die worden toegepast tijdens het renderen van een projectweergave. |
| [getTimescale()](#getTimescale--) | Haalt de `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-))-waarde op die wordt gebruikt om te bepalen hoe de tijdschaal (indien aanwezig) wordt gerenderd wanneer het project wordt opgeslagen in een grafisch formaat. |
| [getTimescaleFitBehavior()](#getTimescaleFitBehavior--) | Haalt een gedrag op dat bepaalt hoe het rechteruiteinde van de tijdschaal wordt uitgelijnd met het einde van de pagina. |
| [getUseGradientBrush()](#getUseGradientBrush--) | Haalt een waarde op die aangeeft of een gradient penseel moet worden gebruikt bij het renderen van een Gantt-diagram. |
| [getView()](#getView--) | Haalt een lijst met de weergavekolommen op die moeten worden gerenderd ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |
| [getViewSettings()](#getViewSettings--) | Haalt een weergave (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) op om te renderen. |
| [isPortrait()](#isPortrait--) | Haalt een waarde op die aangeeft of de paginarichting portret is; retourneert false als de paginarichting landschap is. |
| [setBarStyles(List&lt;BarStyle&gt; value)](#setBarStyles-java.util.List-com.aspose.tasks.BarStyle--) | Stelt de lijst in met de instanties van de [BarStyle](../../com.aspose.tasks/barstyle) klasse die verschijnen in de projectweergave. |
| [setCustomPageSize(Dimension2D value)](#setCustomPageSize-java.awt.geom.Dimension2D-) | Stelt de aangepaste paginagrootte in punten in (1 punt = 1/72 inch). |
| [setDrawNonWorkingTime(boolean value)](#setDrawNonWorkingTime-boolean-) | Stelt een waarde in die aangeeft of niet-werkelijke tijd moet worden getekend (standaardwaarde is WAAR). |
| [setEndDate(Date value)](#setEndDate-java.util.Date-) | Stelt een datum in waarop het renderen moet worden beëindigd. |
| [setFitContent(boolean value)](#setFitContent-boolean-) | Stelt een waarde in die aangeeft of de rijhoogte moet worden vergroot om de inhoud te passen. |
| [setGridlines(List&lt;Gridline&gt; value)](#setGridlines-java.util.List-com.aspose.tasks.Gridline--) | Stelt een lijst in met [Gridline](../../com.aspose.tasks/gridline) die verschijnen in de projectweergave. |
| [setLegendDrawingOptions(int value)](#setLegendDrawingOptions-int-) | Stelt een waarde in die bepaalt hoe een legenda moet worden gerenderd. |
| [setLegendItems(PageLegendItem[] value)](#setLegendItems-com.aspose.tasks.PageLegendItem---) | Stelt een array in van PageLegendItem die bepaalt welke balken moeten worden gerenderd in de paginalegenda. |
| [setMarkCriticalTasks(boolean value)](#setMarkCriticalTasks-boolean-) | Stelt een waarde in die aangeeft of kritieke taken in rode kleur moeten worden weergegeven (standaardwaarde is ONWAAR). |
| [setNonWorkingTimeColor(Color value)](#setNonWorkingTimeColor-java.awt.Color-) | Stelt de kleur voor niet-werkelijke tijd in. |
| [setPageSize(int value)](#setPageSize-int-) | Stelt de grootte van de te renderen pagina in (standaardwaarde is PageSize.A4). |
| [setPortrait(boolean value)](#setPortrait-boolean-) | Stelt een waarde in die aangeeft of de paginarichting portret is; retourneert false als de paginarichting landschap is. |
| [setPresentationFormat(int value)](#setPresentationFormat-int-) | Stelt het `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) in waarin het document wordt opgeslagen. |
| [setRenderToSinglePage(boolean value)](#setRenderToSinglePage-boolean-) | Stelt een waarde in die aangeeft of een project moet worden gerenderd op één pagina wanneer het project wordt opgeslagen in een grafisch formaat. |
| [setRollUpGanttBars(boolean value)](#setRollUpGanttBars-boolean-) | Stelt een waarde in die aangeeft of subtaken op de samenvattingsbalk gemarkeerd moeten worden. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Stelt de datum in waarop het renderen moet beginnen. |
| [setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value)](#setTaskLinkDrawingCallback-com.aspose.tasks.TaskLinkDrawingCallbackDelegate-) | Stelt een callback in die kan worden gebruikt om enkele aspecten van het renderen van taakkoppelingen aan te passen. |
| [setTextStyles(List&lt;TextStyle&gt; value)](#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--) | Stelt de lijst met tekststijlen in die worden toegepast tijdens het renderen van een projectweergave. |
| [setTimescale(int value)](#setTimescale-int-) | Stelt de `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) waarde in die wordt gebruikt om te bepalen hoe de tijdschaal (indien aanwezig) wordt gerenderd wanneer het project wordt opgeslagen in een grafisch formaat. |
| [setTimescaleFitBehavior(int value)](#setTimescaleFitBehavior-int-) | Stelt een gedrag in dat bepaalt hoe het rechteruiteinde van de tijdschaal wordt uitgelijnd met het einde van de pagina. |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | Stelt een waarde in die aangeeft of een gradient penseel moet worden gebruikt bij het renderen van een Gantt-diagram. |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | Stelt een lijst in met de weergavekolommen die moeten worden gerenderd ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |
| [setViewSettings(View value)](#setViewSettings-com.aspose.tasks.View-) | Stelt een weergave (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) in om te renderen. |
### getBarStyles() {#getBarStyles--}
```
public final List<BarStyle> getBarStyles()
```


Haalt de lijst op van de exemplaren van de [BarStyle](../../com.aspose/tasks/barstyle) klasse die verschijnen in de projectweergave.

**Returns:**
java.util.List&lt;com.aspose.tasks.BarStyle&gt; - de lijst met instanties van de [BarStyle](../../com.aspose.tasks/barstyle) klasse die in de projectweergave verschijnen.
### getCustomPageSize() {#getCustomPageSize--}
```
public final Dimension2D getCustomPageSize()
```


Haalt de aangepaste paginagrootte op in points (1 point = 1/72 inch).

**Returns:**
java.awt.geom.Dimension2D - de aangepaste paginagrootte in punten (1 punt = 1/72 inch).
### getDrawNonWorkingTime() {#getDrawNonWorkingTime--}
```
public final boolean getDrawNonWorkingTime()
```


Haalt een waarde op die aangeeft of niet-werkelijke tijd moet worden getekend (standaardwaarde is TRUE).

**Returns:**
boolean - een waarde die aangeeft of niet-werkelijke tijd moet worden getekend (Standaardwaarde is TRUE).
### getEndDate() {#getEndDate--}
```
public final Date getEndDate()
```


Haalt een datum op waarop het renderen moet worden beëindigd.

**Returns:**
java.util.Date - een datum tot wanneer gerenderd moet worden.
### getFitContent() {#getFitContent--}
```
public final boolean getFitContent()
```


Haalt een waarde op die aangeeft of de rijhoogte moet worden vergroot om de inhoud te passen.

**Returns:**
boolean - een waarde die aangeeft of de rijhoogte moet worden verhoogd om de inhoud te passen.
### getGridlines() {#getGridlines--}
```
public final List<Gridline> getGridlines()
```


Haalt een lijst op van [Gridline](../../com.aspose/tasks/gridline) die verschijnen in de projectweergave.

**Returns:**
java.util.List&lt;com.aspose.tasks.Gridline&gt; - een lijst met [Gridline](../../com.aspose.tasks/gridline) die in de projectweergave verschijnen.
### getLegendDrawingOptions() {#getLegendDrawingOptions--}
```
public final int getLegendDrawingOptions()
```


Haalt een waarde op die bepaalt hoe een legenda moet worden gerenderd. Standaardwaarde is LegendDrawingOptions.OnEveryPage.

Is alleen van toepassing wanneer de Gantt-diagramweergave wordt gerenderd.

**Returns:**
int - een waarde die bepaalt hoe een legenda moet worden gerenderd.
### getLegendItems() {#getLegendItems--}
```
public final PageLegendItem[] getLegendItems()
```


Haalt een array op van PageLegendItem die bepalen welke balken in de paginalegenda moeten worden gerenderd. Indien null, worden de standaarditems gerenderd.

Is alleen van toepassing wanneer de Gantt-diagramweergave wordt gerenderd.

**Returns:**
com.aspose.tasks.PageLegendItem[] - een array van PageLegendItem die bepalen welke balken in de paginalegenda moeten worden gerenderd.
### getMarkCriticalTasks() {#getMarkCriticalTasks--}
```
public final boolean getMarkCriticalTasks()
```


Haalt een waarde op die aangeeft of kritieke taken in rode kleur moeten worden weergegeven (standaardwaarde is FALSE).

**Returns:**
boolean - een waarde die aangeeft of kritieke taken in rode kleur moeten worden weergegeven (Standaardwaarde is FALSE).
### getNonWorkingTimeColor() {#getNonWorkingTimeColor--}
```
public final Color getNonWorkingTimeColor()
```


Haalt de kleur van niet-werkelijke tijd op.

**Returns:**
java.awt.Color - de kleur voor niet-werkelijke tijd.
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Haalt het aantal pagina's van het project op.

**Returns:**
int - het aantal pagina's van het project.
### getPageSize() {#getPageSize--}
```
public final int getPageSize()
```


Haalt de grootte van de te renderen pagina op (standaardwaarde is PageSize.A4).

**Returns:**
int - de grootte van de te renderen pagina (Standaardwaarde is PageSize.A4).
### getPresentationFormat() {#getPresentationFormat--}
```
public final int getPresentationFormat()
```


Haalt het `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) op waarin het document wordt opgeslagen.

**Returns:**
int - de `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) waarin het document wordt opgeslagen.
### getRenderToSinglePage() {#getRenderToSinglePage--}
```
public final boolean getRenderToSinglePage()
```


Haalt een waarde op die aangeeft of een project moet worden gerenderd op één pagina wanneer het project wordt opgeslagen in een grafisch formaat. De paginagrootte wordt aangepast zodat het gerenderde project op één pagina past.

**Returns:**
boolean - een waarde die aangeeft of een project moet worden gerenderd naar één pagina wanneer het project wordt opgeslagen in grafisch formaat.
### getRollUpGanttBars() {#getRollUpGanttBars--}
```
public final boolean getRollUpGanttBars()
```


Haalt een waarde op die aangeeft of subtaken op de samenvattingstaakbalk gemarkeerd moeten worden. Voor subtaken geeft het Rollup‑veld aan of informatie over de Gantt‑balken van de subtaak wordt opgehoogd naar de samenvattingstaakbalk. Voor samenvattingstaken geeft het Rollup‑veld aan of de samenvattingstaakbalk opgehoogde balken weergeeft. U moet het Rollup‑veld voor samenvattingstaken op Ja instellen zodat subtaken naar hen worden opgehoogd.

--------------------

Is alleen van toepassing wanneer de Gantt-diagramweergave wordt gerenderd.

**Returns:**
boolean - een waarde die aangeeft of subtaken op de samenvattingstaakbalk gemarkeerd moeten worden.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


Haalt de datum op vanaf wanneer gerenderd moet worden.

**Returns:**
java.util.Date - de datum vanaf wanneer gerenderd moet worden.
### getTaskLinkDrawingCallback() {#getTaskLinkDrawingCallback--}
```
public final TaskLinkDrawingCallbackDelegate getTaskLinkDrawingCallback()
```


Haalt een callback op die kan worden gebruikt om enkele aspecten van het renderen van taaklinks aan te passen.

Is alleen van toepassing wanneer de Gantt-diagramweergave wordt gerenderd.

**Returns:**
[TaskLinkDrawingCallbackDelegate](../../com.aspose.tasks/tasklinkdrawingcallbackdelegate) - a callback that can be used to customize some aspects of task links rendering.
### getTextStyles() {#getTextStyles--}
```
public final List<TextStyle> getTextStyles()
```


Haalt de lijst met tekststijlen op die worden toegepast tijdens het renderen van een projectweergave.

--------------------

Deze stijlen overschrijven de stijlen die zijn gedefinieerd met GanttCharView.setTextStyles.

**Returns:**
java.util.List&lt;com.aspose.tasks.TextStyle&gt; - de lijst met tekststijlen die worden toegepast tijdens het renderen van een projectweergave.
### getTimescale() {#getTimescale--}
```
public final int getTimescale()
```


Haalt de `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-))-waarde op die wordt gebruikt om te bepalen hoe de tijdschaal (indien aanwezig) wordt gerenderd wanneer het project wordt opgeslagen in een grafisch formaat.

**Returns:**
int - de `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) waarde die wordt gebruikt om te bepalen hoe de tijdschaal (indien aanwezig) wordt gerenderd wanneer het project wordt opgeslagen in een grafisch formaat.
### getTimescaleFitBehavior() {#getTimescaleFitBehavior--}
```
public final int getTimescaleFitBehavior()
```


Haalt een gedrag op dat bepaalt hoe het rechteruiteinde van de tijdschaal wordt uitgelijnd met het einde van de pagina.

**Returns:**
int - een gedrag dat bepaalt hoe het rechteruiteinde van de tijdschaal wordt uitgelijnd met het einde van de pagina.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


Haalt een waarde op die aangeeft of een gradient penseel moet worden gebruikt bij het renderen van een Gantt-diagram.

--------------------

Is alleen van toepassing wanneer de Gantt-diagramweergave wordt gerenderd.

**Returns:**
boolean - een waarde die aangeeft of een gradient‑kwast moet worden gebruikt bij het renderen van een Gantt‑diagram.
### getView() {#getView--}
```
public final ProjectView getView()
```


Haalt een lijst op van de weergavekolommen die moeten worden gerenderd ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). Indien niet ingesteld, worden alleen taak‑ID’s, taaknamen, start‑ en einddatums gerenderd. Als zowel View‑ als `ViewSettings`([getViewSettings()](../../com.aspose.tasks/saveoptions\#getViewSettings--)/[setViewSettings(View)](../../com.aspose.tasks/saveoptions\#setViewSettings-View-))‑eigenschappen zijn ingesteld, hebben kolommen van View voorrang op kolommen van ViewSettings.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns to render ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)).
### getViewSettings() {#getViewSettings--}
```
public final View getViewSettings()
```


Haalt een weergave (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) op om te renderen. U kunt deze optie gebruiken om expliciet op te geven welke weergave moet worden opgeslagen als PDF, HTML of afbeelding. Als deze eigenschap is ingesteld, wordt de eigenschap [PresentationFormat](../../com.aspose.tasks/presentationformat) genegeerd wanneer het project wordt opgeslagen. De weergave moet afkomstig zijn van een van de volgende schermen ((`Aspose.Tasks.View.Screen`([View.getScreen()](../../com.aspose.tasks/view\#getScreen--)/[View.setScreen(int)](../../com.aspose.tasks/view\#setScreen-int-)))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage)

**Returns:**
[View](../../com.aspose.tasks/view) - a view (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) to render.
### isPortrait() {#isPortrait--}
```
public final boolean isPortrait()
```


Haalt een waarde op die aangeeft of de paginarichting portret is; retourneert false als de paginarichting landschap is.

--------------------

Is niet van toepassing wanneer SaveOptions.getPageSize() == PageSize.DefinedInView. In dat geval wordt [PageSettings.isPortrait()](../../com.aspose.tasks/pagesettings\#isPortrait--) gebruikt. Is niet van toepassing wanneer [getCustomPageSize()](../../com.aspose.tasks/saveoptions\#getCustomPageSize--) is ingesteld.

**Returns:**
boolean - een waarde die aangeeft of de paginarichting portret is; retourneert false als de paginarichting landschap is.
### setBarStyles(List&lt;BarStyle&gt; value) {#setBarStyles-java.util.List-com.aspose.tasks.BarStyle--}
```
public final void setBarStyles(List<BarStyle> value)
```


Stelt de lijst in met de instanties van de [BarStyle](../../com.aspose.tasks/barstyle) klasse die verschijnen in de projectweergave.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.BarStyle&gt; | de lijst met instanties van de [BarStyle](../../com.aspose.tasks/barstyle)‑klasse die verschijnen in de projectweergave. |

### setCustomPageSize(Dimension2D value) {#setCustomPageSize-java.awt.geom.Dimension2D-}
```
public final void setCustomPageSize(Dimension2D value)
```


Stelt de aangepaste paginagrootte in punten in (1 punt = 1/72 inch).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.awt.geom.Dimension2D | de aangepaste paginagrootte in punten (1 punt = 1/72 inch). |

### setDrawNonWorkingTime(boolean value) {#setDrawNonWorkingTime-boolean-}
```
public final void setDrawNonWorkingTime(boolean value)
```


Stelt een waarde in die aangeeft of niet-werkelijke tijd moet worden getekend (standaardwaarde is WAAR).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of niet-werkelijke tijd moet worden getekend (standaardwaarde is TRUE). |

### setEndDate(Date value) {#setEndDate-java.util.Date-}
```
public final void setEndDate(Date value)
```


Stelt een datum in waarop het renderen moet worden beëindigd.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date | een datum waarop het renderen moet worden beëindigd. |

### setFitContent(boolean value) {#setFitContent-boolean-}
```
public final void setFitContent(boolean value)
```


Stelt een waarde in die aangeeft of de rijhoogte moet worden vergroot om de inhoud te passen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of de rijhoogte moet worden vergroot om de inhoud te passen. |

### setGridlines(List&lt;Gridline&gt; value) {#setGridlines-java.util.List-com.aspose.tasks.Gridline--}
```
public final void setGridlines(List<Gridline> value)
```


Stelt een lijst in met [Gridline](../../com.aspose.tasks/gridline) die verschijnen in de projectweergave.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.Gridline&gt; | een lijst met [Gridline](../../com.aspose.tasks/gridline) die verschijnen in de projectweergave. |

### setLegendDrawingOptions(int value) {#setLegendDrawingOptions-int-}
```
public final void setLegendDrawingOptions(int value)
```


Stelt een waarde in die bepaalt hoe een legenda moet worden gerenderd. Standaardwaarde is LegendDrawingOptions.OnEveryPage.

Is alleen van toepassing wanneer de Gantt-diagramweergave wordt gerenderd.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een waarde die bepaalt hoe een legenda moet worden gerenderd. |

### setLegendItems(PageLegendItem[] value) {#setLegendItems-com.aspose.tasks.PageLegendItem---}
```
public final void setLegendItems(PageLegendItem[] value)
```


Stelt een array van PageLegendItem in die bepaalt welke balken in de paginalegenda moeten worden gerenderd. Indien null, worden de standaarditems gerenderd.

Is alleen van toepassing wanneer de Gantt-diagramweergave wordt gerenderd.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [PageLegendItem\[\]](../../com.aspose.tasks/pagelegenditem) | een array van PageLegendItem die bepaalt welke balken in de paginalegenda moeten worden gerenderd. |

### setMarkCriticalTasks(boolean value) {#setMarkCriticalTasks-boolean-}
```
public final void setMarkCriticalTasks(boolean value)
```


Stelt een waarde in die aangeeft of kritieke taken in rode kleur moeten worden weergegeven (standaardwaarde is ONWAAR).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of kritieke taken in rode kleur moeten worden weergegeven (standaardwaarde is FALSE). |

### setNonWorkingTimeColor(Color value) {#setNonWorkingTimeColor-java.awt.Color-}
```
public final void setNonWorkingTimeColor(Color value)
```


Stelt de kleur voor niet-werkelijke tijd in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.awt.Color | de kleur van de niet-werkende tijd. |

### setPageSize(int value) {#setPageSize-int-}
```
public final void setPageSize(int value)
```


Stelt de grootte van de te renderen pagina in (standaardwaarde is PageSize.A4).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | de grootte van de te renderen pagina (Standaardwaarde is PageSize.A4). |

### setPortrait(boolean value) {#setPortrait-boolean-}
```
public final void setPortrait(boolean value)
```


Stelt een waarde in die aangeeft of de paginarichting portret is; retourneert false als de paginarichting landschap is.

--------------------

Is niet van toepassing wanneer SaveOptions.PageSize == Visualization.PageSize.DefinedInView. In dit geval wordt [PageSettings.setPortrait(boolean)](../../com.aspose.tasks/pagesettings\#setPortrait-boolean-) gebruikt. Is niet van toepassing wanneer [getCustomPageSize()](../../com.aspose.tasks/saveoptions\#getCustomPageSize--) is ingesteld.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of de paginarichting portret is; retourneert false als de paginarichting landschap is. |

### setPresentationFormat(int value) {#setPresentationFormat-int-}
```
public final void setPresentationFormat(int value)
```


Stelt het `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) in waarin het document wordt opgeslagen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | int | de `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) waarin het document wordt opgeslagen. |

### setRenderToSinglePage(boolean value) {#setRenderToSinglePage-boolean-}
```
public final void setRenderToSinglePage(boolean value)
```


Stelt een waarde in die aangeeft of een project moet worden gerenderd naar één pagina wanneer het project wordt opgeslagen in grafisch formaat. De paginagrootte wordt aangepast zodat het gerenderde project op één pagina past.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of een project moet worden gerenderd naar één pagina wanneer het project wordt opgeslagen in grafisch formaat. |

### setRollUpGanttBars(boolean value) {#setRollUpGanttBars-boolean-}
```
public final void setRollUpGanttBars(boolean value)
```


Stelt een waarde in die aangeeft of subtaken op de samenvattingsbalk gemarkeerd moeten worden. Voor subtaken geeft het Rollup‑veld aan of informatie over de Gantt‑balken van de subtaak wordt opgeteld naar de samenvattingsbalk. Voor samenvattende taken geeft het Rollup‑veld aan of de samenvattingsbalk opgetelde balken weergeeft. Het Rollup‑veld voor samenvattende taken moet op Ja staan om subtaken naar hen op te tellen.

--------------------

Is alleen van toepassing wanneer de Gantt-diagramweergave wordt gerenderd.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of subtaken op de samenvattingsbalk gemarkeerd moeten worden. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


Stelt de datum in waarop het renderen moet beginnen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date | de datum vanaf wanneer gerenderd moet worden. |

### setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value) {#setTaskLinkDrawingCallback-com.aspose.tasks.TaskLinkDrawingCallbackDelegate-}
```
public final void setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value)
```


Stelt een callback in die kan worden gebruikt om enkele aspecten van het renderen van taakkoppelingen aan te passen.

Is alleen van toepassing wanneer de Gantt-diagramweergave wordt gerenderd.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [TaskLinkDrawingCallbackDelegate](../../com.aspose.tasks/tasklinkdrawingcallbackdelegate) | een callback die kan worden gebruikt om enkele aspecten van het renderen van taakkoppelingen aan te passen. |

### setTextStyles(List&lt;TextStyle&gt; value) {#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--}
```
public final void setTextStyles(List<TextStyle> value)
```


Stelt de lijst met tekststijlen in die worden toegepast tijdens het renderen van een projectweergave.

--------------------

Deze stijlen overschrijven de stijlen die zijn gedefinieerd met GanttCharView.setTextStyles.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.List&lt;com.aspose.tasks.TextStyle&gt; | de lijst met tekststijlen die worden toegepast tijdens het renderen van een projectweergave. |

### setTimescale(int value) {#setTimescale-int-}
```
public final void setTimescale(int value)
```


Stelt de `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) waarde in die wordt gebruikt om te bepalen hoe de tijdschaal (indien aanwezig) wordt gerenderd wanneer het project wordt opgeslagen in een grafisch formaat.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | int | de `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) waarde die wordt gebruikt om te bepalen hoe de tijdschaal (indien aanwezig) wordt gerenderd wanneer het project wordt opgeslagen in grafisch formaat. |

### setTimescaleFitBehavior(int value) {#setTimescaleFitBehavior-int-}
```
public final void setTimescaleFitBehavior(int value)
```


Stelt een gedrag in dat bepaalt hoe het rechteruiteinde van de tijdschaal wordt uitgelijnd met het einde van de pagina.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een gedrag dat bepaalt hoe het rechteruiteinde van de tijdschaal wordt uitgelijnd met het einde van de pagina. |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


Stelt een waarde in die aangeeft of een gradient penseel moet worden gebruikt bij het renderen van een Gantt-diagram.

--------------------

Is alleen van toepassing wanneer de Gantt-diagramweergave wordt gerenderd.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of een gradient‑kwast moet worden gebruikt bij het renderen van een Gantt‑diagram. |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


Stelt een lijst in met de weergavekolommen die moeten worden gerenderd ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). Indien niet ingesteld, worden alleen taak‑ID's, taaknamen, start‑ en einddatums gerenderd. Als zowel View‑ als `ViewSettings`([getViewSettings()](../../com.aspose.tasks/saveoptions\#getViewSettings--)/[setViewSettings(View)](../../com.aspose.tasks/saveoptions\#setViewSettings-View-))‑eigenschappen zijn ingesteld, hebben kolommen van View voorrang op kolommen van ViewSettings.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | een lijst met de weergavekolommen die moeten worden gerenderd ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |

### setViewSettings(View value) {#setViewSettings-com.aspose.tasks.View-}
```
public final void setViewSettings(View value)
```


Stelt een weergave (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) in om te renderen. U kunt deze optie gebruiken om expliciet op te geven welke weergave moet worden opgeslagen in PDF-, HTML- of afbeeldingsformaten. Als deze eigenschap is ingesteld, wordt de [PresentationFormat](../../com.aspose.tasks/presentationformat)‑eigenschap genegeerd wanneer het project wordt opgeslagen. De weergave moet afkomstig zijn van een van de volgende schermen ((`Aspose.Tasks.View.Screen`([View.getScreen()](../../com.aspose.tasks/view\#getScreen--)/[View.setScreen(int)](../../com.aspose.tasks/view\#setScreen-int-)))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage)

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [View](../../com.aspose.tasks/view) | een weergave (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) om te renderen. |

