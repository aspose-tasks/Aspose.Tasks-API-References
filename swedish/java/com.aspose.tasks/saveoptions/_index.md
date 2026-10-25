---
title: "SaveOptions"
second_title: "Aspose.Tasks for Java API-referens"
description: "Detta är en abstrakt basklass för klasser som låter användaren ange ytterligare alternativ när ett projekt sparas i ett specifikt format."
type: docs
weight: 274
url: /sv/java/com.aspose.tasks/saveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public abstract class SaveOptions extends SimpleSaveOptions
```

Detta är en abstrakt basklass för klasser som låter användaren ange ytterligare alternativ när ett projekt sparas i ett specifikt format.

--------------------

En instans av någon avledd klass från SaveOptions‑klassen skickas till ström‑Save eller sträng‑Save‑överladdningarna så att användaren kan definiera anpassade alternativ när ett dokument sparas.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getBarStyles()](#getBarStyles--) | Hämtar listan över instanserna av klassen [BarStyle](../../com.aspose/tasks/barstyle) som visas i projektvyn. |
| [getCustomPageSize()](#getCustomPageSize--) | Hämtar den anpassade sidstorleken i punkter (1 punkt = 1/72 tum). |
| [getDrawNonWorkingTime()](#getDrawNonWorkingTime--) | Hämtar ett värde som indikerar om icke-arbetstid ska ritas (Standardvärdet är TRUE). |
| [getEndDate()](#getEndDate--) | Hämtar ett datum att slutföra rendering till. |
| [getFitContent()](#getFitContent--) | Hämtar ett värde som indikerar om radhöjden ska ökas för att passa innehållet. |
| [getGridlines()](#getGridlines--) | Hämtar en lista över [Gridline](../../com.aspose/tasks/gridline) som visas i projektvyn. |
| [getLegendDrawingOptions()](#getLegendDrawingOptions--) | Hämtar ett värde som definierar hur en legend ska renderas. |
| [getLegendItems()](#getLegendItems--) | Hämtar en array av PageLegendItem som definierar vilka staplar som ska renderas i sidlegenden. |
| [getMarkCriticalTasks()](#getMarkCriticalTasks--) | Hämtar ett värde som indikerar om kritiska uppgifter ska visas i röd färg (Standardvärdet är FALSE). |
| [getNonWorkingTimeColor()](#getNonWorkingTimeColor--) | Hämtar färgen för icke-arbetstid. |
| [getPageCount()](#getPageCount--) | Hämtar antalet sidor i projektet. |
| [getPageSize()](#getPageSize--) | Hämtar sidans storlek som ska renderas (Standardvärdet är PageSize.A4). |
| [getPresentationFormat()](#getPresentationFormat--) | Hämtar `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) i vilket dokumentet kommer att sparas. |
| [getRenderToSinglePage()](#getRenderToSinglePage--) | Hämtar ett värde som indikerar om ett projekt ska renderas till en enda sida när projektet sparas i grafiskt format. |
| [getRollUpGanttBars()](#getRollUpGanttBars--) | Hämtar ett värde som indikerar om deluppgifter på sammanfattningsradens stapel ska markeras. |
| [getStartDate()](#getStartDate--) | Hämtar datumet att börja rendera från. |
| [getTaskLinkDrawingCallback()](#getTaskLinkDrawingCallback--) | Hämtar en återuppringning som kan användas för att anpassa vissa aspekter av renderingen av uppgiftslänkar. |
| [getTextStyles()](#getTextStyles--) | Hämtar listan med textstilar som tillämpas under rendering av en projektvy. |
| [getTimescale()](#getTimescale--) | Hämtar `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-))‑värdet som används för att styra hur tidslinjen (om den finns) renderas när projektet sparas i grafiskt format. |
| [getTimescaleFitBehavior()](#getTimescaleFitBehavior--) | Hämtar ett beteende som definierar hur den högra änden av tidslinjen ska justeras med sidans slut. |
| [getUseGradientBrush()](#getUseGradientBrush--) | Hämtar ett värde som indikerar om en gradientpensel ska användas vid rendering av Gantt-diagram. |
| [getView()](#getView--) | Hämtar en lista över vykolumnerna som ska renderas ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |
| [getViewSettings()](#getViewSettings--) | Hämtar en vy (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) att rendera. |
| [isPortrait()](#isPortrait--) | Hämtar ett värde som indikerar om sidorienteringen är stående; returnerar false om sidorienteringen är liggande. |
| [setBarStyles(List&lt;BarStyle&gt; value)](#setBarStyles-java.util.List-com.aspose.tasks.BarStyle--) | Ställer in listan med instanser av klassen [BarStyle](../../com.aspose.tasks/barstyle) som visas i projektvyn. |
| [setCustomPageSize(Dimension2D value)](#setCustomPageSize-java.awt.geom.Dimension2D-) | Ställer in den anpassade sidstorleken i punkter (1 punkt = 1/72 tum). |
| [setDrawNonWorkingTime(boolean value)](#setDrawNonWorkingTime-boolean-) | Ställer in ett värde som indikerar om icke-arbetstid ska ritas (standardvärdet är SANT). |
| [setEndDate(Date value)](#setEndDate-java.util.Date-) | Ställer in ett datum att avsluta renderingen till. |
| [setFitContent(boolean value)](#setFitContent-boolean-) | Ställer in ett värde som indikerar om radhöjden ska ökas för att passa innehållet. |
| [setGridlines(List&lt;Gridline&gt; value)](#setGridlines-java.util.List-com.aspose.tasks.Gridline--) | Ställer in en lista med [Gridline](../../com.aspose.tasks/gridline) som visas i projektvyn. |
| [setLegendDrawingOptions(int value)](#setLegendDrawingOptions-int-) | Ställer in ett värde som definierar hur en förklaring ska renderas. |
| [setLegendItems(PageLegendItem[] value)](#setLegendItems-com.aspose.tasks.PageLegendItem---) | Ställer in en array av PageLegendItem som definierar vilka staplar som ska renderas i sidans förklaring. |
| [setMarkCriticalTasks(boolean value)](#setMarkCriticalTasks-boolean-) | Ställer in ett värde som indikerar om kritiska uppgifter ska visas i röd färg (standardvärdet är FALSKT). |
| [setNonWorkingTimeColor(Color value)](#setNonWorkingTimeColor-java.awt.Color-) | Ställer in färgen för icke-arbetstid. |
| [setPageSize(int value)](#setPageSize-int-) | Ställer in sidans storlek som ska renderas (standardvärdet är PageSize.A4). |
| [setPortrait(boolean value)](#setPortrait-boolean-) | Ställer in ett värde som indikerar om sidorienteringen är stående; returnerar false om sidorienteringen är liggande. |
| [setPresentationFormat(int value)](#setPresentationFormat-int-) | Ställer in `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) i vilket dokumentet kommer att sparas. |
| [setRenderToSinglePage(boolean value)](#setRenderToSinglePage-boolean-) | Ställer in ett värde som indikerar om ett projekt ska renderas till en enda sida när projektet sparas i grafiskt format. |
| [setRollUpGanttBars(boolean value)](#setRollUpGanttBars-boolean-) | Ställer in ett värde som indikerar om deluppgifter på sammanfattningsradens stapel ska markeras. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Ställer in datumet att börja rendera från. |
| [setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value)](#setTaskLinkDrawingCallback-com.aspose.tasks.TaskLinkDrawingCallbackDelegate-) | Ställer in en callback som kan användas för att anpassa vissa aspekter av rendering av uppgiftslänkar. |
| [setTextStyles(List&lt;TextStyle&gt; value)](#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--) | Ställer in listan med textstilar som tillämpas under rendering av en projektvy. |
| [setTimescale(int value)](#setTimescale-int-) | Ställer in `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) värdet som används för att kontrollera hur tidslinjen (om den finns) renderas när projektet sparas i grafiskt format. |
| [setTimescaleFitBehavior(int value)](#setTimescaleFitBehavior-int-) | Ställer in ett beteende som definierar hur den högra änden av tidslinjen ska justeras med sidans slut. |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | Ställer in ett värde som indikerar om en gradientpensel ska användas vid rendering av Gantt-diagram. |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | Ställer in en lista med vykolumner som ska renderas ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |
| [setViewSettings(View value)](#setViewSettings-com.aspose.tasks.View-) | Ställer in en vy (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) för att rendera. |
### getBarStyles() {#getBarStyles--}
```
public final List<BarStyle> getBarStyles()
```


Hämtar listan över instanserna av klassen [BarStyle](../../com.aspose/tasks/barstyle) som visas i projektvyn.

**Returns:**
java.util.List&lt;com.aspose.tasks.BarStyle&gt; - listan med instanser av klassen [BarStyle](../../com.aspose.tasks/barstyle) som visas i projektvyn.
### getCustomPageSize() {#getCustomPageSize--}
```
public final Dimension2D getCustomPageSize()
```


Hämtar den anpassade sidstorleken i punkter (1 punkt = 1/72 tum).

**Returns:**
java.awt.geom.Dimension2D - den anpassade sidstorleken i punkter (1 punkt = 1/72 tum).
### getDrawNonWorkingTime() {#getDrawNonWorkingTime--}
```
public final boolean getDrawNonWorkingTime()
```


Hämtar ett värde som indikerar om icke-arbetstid ska ritas (Standardvärdet är TRUE).

**Returns:**
boolean - ett värde som indikerar om icke-arbetstid ska ritas (Standardvärdet är TRUE).
### getEndDate() {#getEndDate--}
```
public final Date getEndDate()
```


Hämtar ett datum att slutföra rendering till.

**Returns:**
java.util.Date - ett datum att avsluta rendering till.
### getFitContent() {#getFitContent--}
```
public final boolean getFitContent()
```


Hämtar ett värde som indikerar om radhöjden ska ökas för att passa innehållet.

**Returns:**
boolean - ett värde som indikerar om radhöjden ska ökas för att passa innehållet.
### getGridlines() {#getGridlines--}
```
public final List<Gridline> getGridlines()
```


Hämtar en lista över [Gridline](../../com.aspose/tasks/gridline) som visas i projektvyn.

**Returns:**
java.util.List&lt;com.aspose.tasks.Gridline&gt; - en lista med [Gridline](../../com.aspose.tasks/gridline) som visas i projektvyn.
### getLegendDrawingOptions() {#getLegendDrawingOptions--}
```
public final int getLegendDrawingOptions()
```


Hämtar ett värde som definierar hur en legend ska renderas. Standardvärdet är LegendDrawingOptions.OnEveryPage.

Gäller endast när Gantt-diagramvyn renderas.

**Returns:**
int - ett värde som definierar hur en legend ska renderas.
### getLegendItems() {#getLegendItems--}
```
public final PageLegendItem[] getLegendItems()
```


Hämtar en array av PageLegendItem som definierar vilka staplar som ska renderas i sidlegenden. Om null renderas standardobjekten.

Gäller endast när Gantt-diagramvyn renderas.

**Returns:**
com.aspose.tasks.PageLegendItem[] - en array av PageLegendItem som definierar vilka staplar som ska renderas i sidlegenden.
### getMarkCriticalTasks() {#getMarkCriticalTasks--}
```
public final boolean getMarkCriticalTasks()
```


Hämtar ett värde som indikerar om kritiska uppgifter ska visas i röd färg (Standardvärdet är FALSE).

**Returns:**
boolean - ett värde som indikerar om kritiska uppgifter ska visas i röd färg (Standardvärdet är FALSE).
### getNonWorkingTimeColor() {#getNonWorkingTimeColor--}
```
public final Color getNonWorkingTimeColor()
```


Hämtar färgen för icke-arbetstid.

**Returns:**
java.awt.Color - färgen för icke-arbetstid.
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Hämtar antalet sidor i projektet.

**Returns:**
int - antalet sidor i projektet.
### getPageSize() {#getPageSize--}
```
public final int getPageSize()
```


Hämtar sidans storlek som ska renderas (Standardvärdet är PageSize.A4).

**Returns:**
int - storleken på sidan som ska renderas (Standardvärdet är PageSize.A4).
### getPresentationFormat() {#getPresentationFormat--}
```
public final int getPresentationFormat()
```


Hämtar `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) i vilket dokumentet kommer att sparas.

**Returns:**
int - `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) i vilket format dokumentet kommer att sparas.
### getRenderToSinglePage() {#getRenderToSinglePage--}
```
public final boolean getRenderToSinglePage()
```


Hämtar ett värde som indikerar om ett projekt ska renderas till en enda sida när projektet sparas i grafiskt format. Sidstorleken kommer att ändras så att det renderade projektet får plats på en sida.

**Returns:**
boolean - ett värde som indikerar om ett projekt ska renderas till en enda sida när projektet sparas i grafiskt format.
### getRollUpGanttBars() {#getRollUpGanttBars--}
```
public final boolean getRollUpGanttBars()
```


Hämtar ett värde som indikerar om deluppgifter på sammanfattningsuppgiftens stapel ska markeras. För deluppgifter indikerar fältet Rollup om information på deluppgiftens Gantt-staplar kommer att rullas upp till sammanfattningsuppgiftens stapel. För sammanfattningsuppgifter indikerar fältet Rollup om stapeln för sammanfattningsuppgiften visar upprullade staplar. Du måste ha fältet Rollup för sammanfattningsuppgifter satt till Ja för att någon deluppgift ska rullas upp till dem.

--------------------

Gäller endast när Gantt-diagramvyn renderas.

**Returns:**
boolean - ett värde som indikerar om deluppgifter på sammanfattningsuppgiftens stapel ska markeras.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


Hämtar datumet att börja rendera från.

**Returns:**
java.util.Date - datumet att börja rendera från.
### getTaskLinkDrawingCallback() {#getTaskLinkDrawingCallback--}
```
public final TaskLinkDrawingCallbackDelegate getTaskLinkDrawingCallback()
```


Hämtar en återuppringning som kan användas för att anpassa vissa aspekter av renderingen av uppgiftslänkar.

Gäller endast när Gantt-diagramvyn renderas.

**Returns:**
[TaskLinkDrawingCallbackDelegate](../../com.aspose.tasks/tasklinkdrawingcallbackdelegate) - a callback that can be used to customize some aspects of task links rendering.
### getTextStyles() {#getTextStyles--}
```
public final List<TextStyle> getTextStyles()
```


Hämtar listan med textstilar som tillämpas under rendering av en projektvy.

--------------------

Dessa stilar åsidosätter stilar som definierats med GanttCharView.setTextStyles.

**Returns:**
java.util.List&lt;com.aspose.tasks.TextStyle&gt; - listan med textstilar som tillämpas under rendering av en projektvy.
### getTimescale() {#getTimescale--}
```
public final int getTimescale()
```


Hämtar `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-))‑värdet som används för att styra hur tidslinjen (om den finns) renderas när projektet sparas i grafiskt format.

**Returns:**
int - `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-))‑värdet som används för att styra hur tidslinjen (om den finns) renderas när projektet sparas i grafiskt format.
### getTimescaleFitBehavior() {#getTimescaleFitBehavior--}
```
public final int getTimescaleFitBehavior()
```


Hämtar ett beteende som definierar hur den högra änden av tidslinjen ska justeras med sidans slut.

**Returns:**
int - ett beteende som definierar hur den högra änden av tidslinjen ska justeras med sidans slut.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


Hämtar ett värde som indikerar om en gradientpensel ska användas vid rendering av Gantt-diagram.

--------------------

Gäller endast när Gantt-diagramvyn renderas.

**Returns:**
boolean - ett värde som indikerar om en gradientpensel ska användas vid rendering av Gantt-diagram.
### getView() {#getView--}
```
public final ProjectView getView()
```


Hämtar en lista med vykolumner som ska renderas ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). Om den inte är angiven renderas endast uppgifts‑ID:n, uppgiftsnamnen, start och slut. Om både View och `ViewSettings`([getViewSettings()](../../com.aspose.tasks/saveoptions\#getViewSettings--)/[setViewSettings(View)](../../com.aspose.tasks/saveoptions\#setViewSettings-View-))‑egenskaperna är satta, åsidosätter kolumner från View kolumner från ViewSettings.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns to render ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)).
### getViewSettings() {#getViewSettings--}
```
public final View getViewSettings()
```


Hämtar en vy (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) att rendera. Du kan använda detta alternativ för att explicit ange vilken vy som ska sparas till PDF-, HTML- eller Bildformat. Om denna egenskap är satt ignoreras [PresentationFormat](../../com.aspose.tasks/presentationformat)‑egenskapen när projektet sparas. Vyn ska vara från en av följande skärmar ((`Aspose.Tasks.View.Screen`([View.getScreen()](../../com.aspose.tasks/view\#getScreen--)/[View.setScreen(int)](../../com.aspose.tasks/view\#setScreen-int-)))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage)

**Returns:**
[View](../../com.aspose.tasks/view) - a view (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) to render.
### isPortrait() {#isPortrait--}
```
public final boolean isPortrait()
```


Hämtar ett värde som indikerar om sidorienteringen är stående; returnerar false om sidorienteringen är liggande.

--------------------

Gäller inte när SaveOptions.getPageSize() == PageSize.DefinedInView. I detta fall används [PageSettings.isPortrait()](../../com.aspose.tasks/pagesettings\#isPortrait--) istället. Gäller inte när [getCustomPageSize()](../../com.aspose.tasks/saveoptions\#getCustomPageSize--) är satt.

**Returns:**
boolean - ett värde som indikerar om sidorienteringen är stående; returnerar false om sidorienteringen är liggande.
### setBarStyles(List&lt;BarStyle&gt; value) {#setBarStyles-java.util.List-com.aspose.tasks.BarStyle--}
```
public final void setBarStyles(List<BarStyle> value)
```


Ställer in listan med instanser av klassen [BarStyle](../../com.aspose.tasks/barstyle) som visas i projektvyn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.BarStyle&gt; | listan med instanser av klassen [BarStyle](../../com.aspose.tasks/barstyle) som visas i projektvyn. |

### setCustomPageSize(Dimension2D value) {#setCustomPageSize-java.awt.geom.Dimension2D-}
```
public final void setCustomPageSize(Dimension2D value)
```


Ställer in den anpassade sidstorleken i punkter (1 punkt = 1/72 tum).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.awt.geom.Dimension2D | den anpassade sidstorleken i punkter (1 punkt = 1/72 tum). |

### setDrawNonWorkingTime(boolean value) {#setDrawNonWorkingTime-boolean-}
```
public final void setDrawNonWorkingTime(boolean value)
```


Ställer in ett värde som indikerar om icke-arbetstid ska ritas (standardvärdet är SANT).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om icke-arbetstid ska ritas (standardvärdet är SANT). |

### setEndDate(Date value) {#setEndDate-java.util.Date-}
```
public final void setEndDate(Date value)
```


Ställer in ett datum att avsluta renderingen till.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date | ett datum att avsluta rendering till. |

### setFitContent(boolean value) {#setFitContent-boolean-}
```
public final void setFitContent(boolean value)
```


Ställer in ett värde som indikerar om radhöjden ska ökas för att passa innehållet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om radhöjden ska ökas för att passa dess innehåll. |

### setGridlines(List&lt;Gridline&gt; value) {#setGridlines-java.util.List-com.aspose.tasks.Gridline--}
```
public final void setGridlines(List<Gridline> value)
```


Ställer in en lista med [Gridline](../../com.aspose.tasks/gridline) som visas i projektvyn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.Gridline&gt; | en lista med [Gridline](../../com.aspose.tasks/gridline) som visas i projektvyn. |

### setLegendDrawingOptions(int value) {#setLegendDrawingOptions-int-}
```
public final void setLegendDrawingOptions(int value)
```


Ställer in ett värde som definierar hur en legend ska renderas. Standardvärdet är LegendDrawingOptions.OnEveryPage.

Gäller endast när Gantt-diagramvyn renderas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | ett värde som definierar hur en legend ska renderas. |

### setLegendItems(PageLegendItem[] value) {#setLegendItems-com.aspose.tasks.PageLegendItem---}
```
public final void setLegendItems(PageLegendItem[] value)
```


Ställer in en array av PageLegendItem som definierar vilka staplar som ska renderas i sidlegenden. Om null renderas standardobjekten.

Gäller endast när Gantt-diagramvyn renderas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [PageLegendItem\[\]](../../com.aspose.tasks/pagelegenditem) | en array av PageLegendItem som definierar vilka staplar som ska renderas i sidlegenden. |

### setMarkCriticalTasks(boolean value) {#setMarkCriticalTasks-boolean-}
```
public final void setMarkCriticalTasks(boolean value)
```


Ställer in ett värde som indikerar om kritiska uppgifter ska visas i röd färg (standardvärdet är FALSKT).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som anger om kritiska uppgifter ska visas i röd färg (Standardvärdet är FALSE). |

### setNonWorkingTimeColor(Color value) {#setNonWorkingTimeColor-java.awt.Color-}
```
public final void setNonWorkingTimeColor(Color value)
```


Ställer in färgen för icke-arbetstid.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.awt.Color | färgen för icke-arbetstid. |

### setPageSize(int value) {#setPageSize-int-}
```
public final void setPageSize(int value)
```


Ställer in sidans storlek som ska renderas (standardvärdet är PageSize.A4).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | storleken på sidan som ska renderas (Standardvärdet är PageSize.A4). |

### setPortrait(boolean value) {#setPortrait-boolean-}
```
public final void setPortrait(boolean value)
```


Ställer in ett värde som indikerar om sidorienteringen är stående; returnerar false om sidorienteringen är liggande.

--------------------

Gäller inte när SaveOptions.PageSize == Visualization.PageSize.DefinedInView. I detta fall används [PageSettings.setPortrait(boolean)](../../com.aspose.tasks/pagesettings\#setPortrait-boolean-) istället. Gäller inte när [getCustomPageSize()](../../com.aspose.tasks/saveoptions\#getCustomPageSize--) är inställd.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om sidorienteringen är stående; returnerar false om sidorienteringen är liggande. |

### setPresentationFormat(int value) {#setPresentationFormat-int-}
```
public final void setPresentationFormat(int value)
```


Ställer in `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) i vilket dokumentet kommer att sparas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | int | den `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) i vilken dokumentet kommer att sparas. |

### setRenderToSinglePage(boolean value) {#setRenderToSinglePage-boolean-}
```
public final void setRenderToSinglePage(boolean value)
```


Ställer in ett värde som anger om ett projekt ska renderas till en enda sida när projektet sparas i grafiskt format. Sidstorleken kommer att ändras så att det renderade projektet får plats på en sida.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som anger om ett projekt ska renderas till en enda sida när projektet sparas i grafiskt format. |

### setRollUpGanttBars(boolean value) {#setRollUpGanttBars-boolean-}
```
public final void setRollUpGanttBars(boolean value)
```


Ställer in ett värde som anger om deluppgifter på sammanfattningsuppgiftens stapel ska markeras. För deluppgifter indikerar Rollup-fältet om information på deluppgiftens Gantt-staplar ska rullas upp till sammanfattningsuppgiftens stapel. För sammanfattningsuppgifter indikerar Rollup-fältet om stapeln för sammanfattningsuppgiften visar upprullade staplar. Du måste ha Rollup-fältet för sammanfattningsuppgifter satt till Ja för att någon deluppgift ska rullas upp till dem.

--------------------

Gäller endast när Gantt-diagramvyn renderas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som anger om deluppgifter på sammanfattningsuppgiftens stapel ska markeras. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


Ställer in datumet att börja rendera från.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date | datumet att börja rendera från. |

### setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value) {#setTaskLinkDrawingCallback-com.aspose.tasks.TaskLinkDrawingCallbackDelegate-}
```
public final void setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value)
```


Ställer in en callback som kan användas för att anpassa vissa aspekter av rendering av uppgiftslänkar.

Gäller endast när Gantt-diagramvyn renderas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [TaskLinkDrawingCallbackDelegate](../../com.aspose.tasks/tasklinkdrawingcallbackdelegate) | en återuppringning som kan användas för att anpassa vissa aspekter av renderingen av uppgiftslänkar. |

### setTextStyles(List&lt;TextStyle&gt; value) {#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--}
```
public final void setTextStyles(List<TextStyle> value)
```


Ställer in listan med textstilar som tillämpas under rendering av en projektvy.

--------------------

Dessa stilar åsidosätter stilar som definierats med GanttCharView.setTextStyles.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.List&lt;com.aspose.tasks.TextStyle&gt; | listan med textstilar som tillämpas under renderingen av en projektvy. |

### setTimescale(int value) {#setTimescale-int-}
```
public final void setTimescale(int value)
```


Ställer in `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) värdet som används för att kontrollera hur tidslinjen (om den finns) renderas när projektet sparas i grafiskt format.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | int | det `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) värdet som används för att styra hur tidslinjen (om den finns) renderas när projektet sparas i grafiskt format. |

### setTimescaleFitBehavior(int value) {#setTimescaleFitBehavior-int-}
```
public final void setTimescaleFitBehavior(int value)
```


Ställer in ett beteende som definierar hur den högra änden av tidslinjen ska justeras med sidans slut.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | ett beteende som definierar hur den högra änden av tidslinjen ska justeras med sidans slut. |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


Ställer in ett värde som indikerar om en gradientpensel ska användas vid rendering av Gantt-diagram.

--------------------

Gäller endast när Gantt-diagramvyn renderas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som anger om en gradientpensel ska användas vid rendering av Gantt-diagram. |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


Ställer in en lista med visningskolumner som ska renderas ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). Om den inte är inställd renderas endast uppgifts‑ID, uppgiftsnamn, start och slut. Om både View och `ViewSettings`([getViewSettings()](../../com.aspose.tasks/saveoptions\#getViewSettings--)/[setViewSettings(View)](../../com.aspose.tasks/saveoptions\#setViewSettings-View-)) egenskaper är satta, åsidosätter kolumner från View kolumner från ViewSettings.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | en lista över vykolumnerna som ska renderas ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |

### setViewSettings(View value) {#setViewSettings-com.aspose.tasks.View-}
```
public final void setViewSettings(View value)
```


Sätter en vy (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) att renderas. Du kan använda detta alternativ för att explicit ange vilken vy som ska sparas till PDF-, HTML- eller Bildformat. Om denna egenskap är satt, ignoreras egenskapen [PresentationFormat](../../com.aspose.tasks/presentationformat) när projektet sparas. Vyn bör vara från en av följande skärmar ((`Aspose.Tasks.View.Screen`([View.getScreen()](../../com.aspose.tasks/view\#getScreen--)/[View.setScreen(int)](../../com.aspose.tasks/view\#setScreen-int-)))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage)

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [View](../../com.aspose.tasks/view) | en vy (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) att renderas. |

