---
title: "SaveOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "Dies ist eine abstrakte Basisklasse für Klassen, die dem Benutzer ermöglichen, zusätzliche Optionen beim Speichern eines Projekts in ein bestimmtes Format anzugeben."
type: docs
weight: 274
url: /de/java/com.aspose.tasks/saveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public abstract class SaveOptions extends SimpleSaveOptions
```

Dies ist eine abstrakte Basisklasse für Klassen, die dem Benutzer ermöglichen, zusätzliche Optionen beim Speichern eines Projekts in ein bestimmtes Format anzugeben.

--------------------

Eine Instanz einer beliebigen von der Klasse SaveOptions abgeleiteten Klasse wird an die Stream‑Save‑ oder String‑Save‑Überladungen übergeben, damit der Benutzer beim Speichern eines Dokuments benutzerdefinierte Optionen festlegen kann.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getBarStyles()](#getBarStyles--) | Gibt die Liste der Instanzen der Klasse [BarStyle](../../com.aspose.tasks/barstyle) zurück, die in der Projektansicht erscheinen. |
| [getCustomPageSize()](#getCustomPageSize--) | Gibt die benutzerdefinierte Seitengröße in Punkten zurück (1 Punkt = 1/72 Zoll). |
| [getDrawNonWorkingTime()](#getDrawNonWorkingTime--) | Gibt einen Wert zurück, der angibt, ob Nichtarbeitszeit gezeichnet werden soll (Standardwert ist TRUE). |
| [getEndDate()](#getEndDate--) | Gibt ein Datum zurück, bis zu dem das Rendering abgeschlossen sein soll. |
| [getFitContent()](#getFitContent--) | Gibt einen Wert zurück, der angibt, ob die Zeilenhöhe erhöht werden soll, um den Inhalt anzupassen. |
| [getGridlines()](#getGridlines--) | Gibt eine Liste von [Gridline](../../com.aspose.tasks/gridline) zurück, die in der Projektansicht erscheinen. |
| [getLegendDrawingOptions()](#getLegendDrawingOptions--) | Gibt einen Wert zurück, der definiert, wie eine Legende gerendert wird. |
| [getLegendItems()](#getLegendItems--) | Gibt ein Array von PageLegendItem zurück, das definiert, welche Balken in der Seitenlegende gerendert werden sollen. |
| [getMarkCriticalTasks()](#getMarkCriticalTasks--) | Gibt einen Wert zurück, der angibt, ob kritische Aufgaben in roter Farbe angezeigt werden sollen (Standardwert ist FALSE). |
| [getNonWorkingTimeColor()](#getNonWorkingTimeColor--) | Gibt die Farbe der Nichtarbeitszeit zurück. |
| [getPageCount()](#getPageCount--) | Ermittelt die Anzahl der Seiten des Projekts. |
| [getPageSize()](#getPageSize--) | Ermittelt die Größe der zu rendernden Seite (Standardwert ist PageSize.A4). |
| [getPresentationFormat()](#getPresentationFormat--) | Ermittelt das `PresentationFormat`([getPresentationFormat()](../../com.aspose/tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose/tasks/saveoptions\#setPresentationFormat-int-)) in dem das Dokument gespeichert wird. |
| [getRenderToSinglePage()](#getRenderToSinglePage--) | Ermittelt einen Wert, der angibt, ob ein Projekt in einer einzelnen Seite gerendert werden soll, wenn das Projekt im grafischen Format gespeichert wird. |
| [getRollUpGanttBars()](#getRollUpGanttBars--) | Ermittelt einen Wert, der angibt, ob Unteraufgaben in der Zusammenfassungsaufgabenleiste markiert werden sollen. |
| [getStartDate()](#getStartDate--) | Ermittelt das Datum, ab dem das Rendern beginnen soll. |
| [getTaskLinkDrawingCallback()](#getTaskLinkDrawingCallback--) | Ermittelt einen Callback, der verwendet werden kann, um einige Aspekte der Darstellung von Aufgabenverknüpfungen anzupassen. |
| [getTextStyles()](#getTextStyles--) | Ermittelt die Liste der Textstile, die während der Darstellung einer Projektansicht angewendet werden. |
| [getTimescale()](#getTimescale--) | Ermittelt den `Timescale`([getTimescale()](../../com.aspose/tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose/tasks/saveoptions\#setTimescale-int-)) Wert, der verwendet wird, um zu steuern, wie die Zeitskala (falls vorhanden) gerendert wird, wenn das Projekt im grafischen Format gespeichert wird. |
| [getTimescaleFitBehavior()](#getTimescaleFitBehavior--) | Ermittelt ein Verhalten, das definiert, wie das rechte Ende der Zeitskala mit dem Seitenende ausgerichtet wird. |
| [getUseGradientBrush()](#getUseGradientBrush--) | Ermittelt einen Wert, der angibt, ob ein Farbverlaufspinsel beim Rendern des Gantt-Diagramms verwendet werden soll. |
| [getView()](#getView--) | Ermittelt eine Liste der Ansichtsspalten, die gerendert werden sollen ([GanttChartColumn](../../com.aspose/tasks/ganttchartcolumn)). |
| [getViewSettings()](#getViewSettings--) | Ermittelt eine Ansicht (`View`([getView()](../../com.aspose/tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose/tasks/saveoptions\#setView-ProjectView-))) zum Rendern. |
| [isPortrait()](#isPortrait--) | Gibt einen Wert zurück, der angibt, ob die Seitenorientierung Hochformat ist; gibt false zurück, wenn die Seitenorientierung Querformat ist. |
| [setBarStyles(List&lt;BarStyle&gt; value)](#setBarStyles-java.util.List-com.aspose.tasks.BarStyle--) | Legt die Liste der Instanzen der Klasse [BarStyle](../../com.aspose/tasks/barstyle) fest, die in der Projektansicht erscheinen. |
| [setCustomPageSize(Dimension2D value)](#setCustomPageSize-java.awt.geom.Dimension2D-) | Legt die benutzerdefinierte Seitengröße in Punkten fest (1 Punkt = 1/72 Zoll). |
| [setDrawNonWorkingTime(boolean value)](#setDrawNonWorkingTime-boolean-) | Legt einen Wert fest, der angibt, ob Nichtarbeitszeit gezeichnet werden soll (Standardwert ist TRUE). |
| [setEndDate(Date value)](#setEndDate-java.util.Date-) | Legt ein Datum fest, bis zu dem das Rendern abgeschlossen sein soll. |
| [setFitContent(boolean value)](#setFitContent-boolean-) | Legt einen Wert fest, der angibt, ob die Zeilenhöhe erhöht werden soll, um den Inhalt anzupassen. |
| [setGridlines(List&lt;Gridline&gt; value)](#setGridlines-java.util.List-com.aspose.tasks.Gridline--) | Legt eine Liste von [Gridline](../../com.aspose/tasks/gridline) fest, die in der Projektansicht erscheinen. |
| [setLegendDrawingOptions(int value)](#setLegendDrawingOptions-int-) | Legt einen Wert fest, der definiert, wie eine Legende gerendert wird. |
| [setLegendItems(PageLegendItem[] value)](#setLegendItems-com.aspose.tasks.PageLegendItem---) | Legt ein Array von PageLegendItem fest, das definiert, welche Balken in der Seitenlegende gerendert werden sollen. |
| [setMarkCriticalTasks(boolean value)](#setMarkCriticalTasks-boolean-) | Legt einen Wert fest, der angibt, ob kritische Aufgaben in roter Farbe angezeigt werden sollen (Standardwert ist FALSE). |
| [setNonWorkingTimeColor(Color value)](#setNonWorkingTimeColor-java.awt.Color-) | Legt die Farbe für Nichtarbeitszeit fest. |
| [setPageSize(int value)](#setPageSize-int-) | Legt die Größe der zu rendernden Seite fest (Standardwert ist PageSize.A4). |
| [setPortrait(boolean value)](#setPortrait-boolean-) | Setzt einen Wert, der angibt, ob die Seitenorientierung Hochformat ist; gibt false zurück, wenn die Seitenorientierung Querformat ist. |
| [setPresentationFormat(int value)](#setPresentationFormat-int-) | Legt das `PresentationFormat`([getPresentationFormat()](../../com.aspose/tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose/tasks/saveoptions\#setPresentationFormat-int-)) fest, in dem das Dokument gespeichert wird. |
| [setRenderToSinglePage(boolean value)](#setRenderToSinglePage-boolean-) | Legt einen Wert fest, der angibt, ob ein Projekt auf einer einzelnen Seite gerendert werden soll, wenn das Projekt im grafischen Format gespeichert wird. |
| [setRollUpGanttBars(boolean value)](#setRollUpGanttBars-boolean-) | Legt einen Wert fest, der angibt, ob Teilaufgaben in der Zusammenfassungsaufgabenleiste markiert werden sollen. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Legt das Datum fest, ab dem gerendert werden soll. |
| [setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value)](#setTaskLinkDrawingCallback-com.aspose.tasks.TaskLinkDrawingCallbackDelegate-) | Legt einen Callback fest, der verwendet werden kann, um einige Aspekte der Darstellung von Aufgabenverknüpfungen anzupassen. |
| [setTextStyles(List&lt;TextStyle&gt; value)](#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--) | Legt die Liste der Textstile fest, die während der Darstellung einer Projektansicht angewendet werden. |
| [setTimescale(int value)](#setTimescale-int-) | Legt den `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) Wert fest, der verwendet wird, um zu steuern, wie die Zeitskala (falls vorhanden) gerendert wird, wenn das Projekt im grafischen Format gespeichert wird. |
| [setTimescaleFitBehavior(int value)](#setTimescaleFitBehavior-int-) | Legt ein Verhalten fest, das definiert, wie das rechte Ende der Zeitskala mit dem Seitenende ausgerichtet wird. |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | Legt einen Wert fest, der angibt, ob ein Farbverlaufspinsel beim Rendern des Gantt-Diagramms verwendet werden soll. |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | Legt eine Liste der Ansichtsspalten fest, die gerendert werden sollen ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |
| [setViewSettings(View value)](#setViewSettings-com.aspose.tasks.View-) | Legt eine Ansicht (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) fest, die gerendert werden soll. |
### getBarStyles() {#getBarStyles--}
```
public final List<BarStyle> getBarStyles()
```


Gibt die Liste der Instanzen der Klasse [BarStyle](../../com.aspose.tasks/barstyle) zurück, die in der Projektansicht erscheinen.

**Returns:**
java.util.List&lt;com.aspose.tasks.BarStyle&gt; – die Liste der Instanzen der Klasse [BarStyle](../../com.aspose.tasks/barstyle), die in der Projektansicht erscheinen.
### getCustomPageSize() {#getCustomPageSize--}
```
public final Dimension2D getCustomPageSize()
```


Gibt die benutzerdefinierte Seitengröße in Punkten zurück (1 Punkt = 1/72 Zoll).

**Returns:**
java.awt.geom.Dimension2D – die benutzerdefinierte Seitengröße in Punkten (1 Punkt = 1/72 Zoll).
### getDrawNonWorkingTime() {#getDrawNonWorkingTime--}
```
public final boolean getDrawNonWorkingTime()
```


Gibt einen Wert zurück, der angibt, ob Nichtarbeitszeit gezeichnet werden soll (Standardwert ist TRUE).

**Returns:**
boolean – ein Wert, der angibt, ob Nichtarbeitszeit gezeichnet werden soll (Standardwert ist TRUE).
### getEndDate() {#getEndDate--}
```
public final Date getEndDate()
```


Gibt ein Datum zurück, bis zu dem das Rendering abgeschlossen sein soll.

**Returns:**
java.util.Date – ein Datum, bis zu dem gerendert werden soll.
### getFitContent() {#getFitContent--}
```
public final boolean getFitContent()
```


Gibt einen Wert zurück, der angibt, ob die Zeilenhöhe erhöht werden soll, um den Inhalt anzupassen.

**Returns:**
boolean – ein Wert, der angibt, ob die Zeilenhöhe erhöht werden soll, um den Inhalt anzupassen.
### getGridlines() {#getGridlines--}
```
public final List<Gridline> getGridlines()
```


Gibt eine Liste von [Gridline](../../com.aspose.tasks/gridline) zurück, die in der Projektansicht erscheinen.

**Returns:**
java.util.List&lt;com.aspose.tasks.Gridline&gt; – eine Liste von [Gridline](../../com.aspose.tasks/gridline), die in der Projektansicht erscheinen.
### getLegendDrawingOptions() {#getLegendDrawingOptions--}
```
public final int getLegendDrawingOptions()
```


Ermittelt einen Wert, der definiert, wie eine Legende gerendert wird. Standardwert ist LegendDrawingOptions.OnEveryPage.

Gilt nur, wenn die Gantt-Diagrammansicht gerendert wird.

**Returns:**
int – ein Wert, der definiert, wie eine Legende gerendert wird.
### getLegendItems() {#getLegendItems--}
```
public final PageLegendItem[] getLegendItems()
```


Ermittelt ein Array von PageLegendItem, das definiert, welche Balken in der Seitenlegende gerendert werden sollen. Wenn null, werden die Standardobjekte gerendert.

Gilt nur, wenn die Gantt-Diagrammansicht gerendert wird.

**Returns:**
com.aspose.tasks.PageLegendItem[] – ein Array von PageLegendItem, das definiert, welche Balken in der Seitenlegende gerendert werden sollen.
### getMarkCriticalTasks() {#getMarkCriticalTasks--}
```
public final boolean getMarkCriticalTasks()
```


Gibt einen Wert zurück, der angibt, ob kritische Aufgaben in roter Farbe angezeigt werden sollen (Standardwert ist FALSE).

**Returns:**
boolean – ein Wert, der angibt, ob kritische Aufgaben in roter Farbe angezeigt werden sollen (Standardwert ist FALSE).
### getNonWorkingTimeColor() {#getNonWorkingTimeColor--}
```
public final Color getNonWorkingTimeColor()
```


Gibt die Farbe der Nichtarbeitszeit zurück.

**Returns:**
java.awt.Color – die Farbe für Nichtarbeitszeit.
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Ermittelt die Anzahl der Seiten des Projekts.

**Returns:**
int – die Anzahl der Seiten des Projekts.
### getPageSize() {#getPageSize--}
```
public final int getPageSize()
```


Ermittelt die Größe der zu rendernden Seite (Standardwert ist PageSize.A4).

**Returns:**
int – die Größe der zu rendernden Seite (Standardwert ist PageSize.A4).
### getPresentationFormat() {#getPresentationFormat--}
```
public final int getPresentationFormat()
```


Ermittelt das `PresentationFormat`([getPresentationFormat()](../../com.aspose/tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose/tasks/saveoptions\#setPresentationFormat-int-)) in dem das Dokument gespeichert wird.

**Returns:**
int - das `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) in dem das Dokument gespeichert wird.
### getRenderToSinglePage() {#getRenderToSinglePage--}
```
public final boolean getRenderToSinglePage()
```


Gibt einen Wert zurück, der angibt, ob ein Projekt auf einer einzigen Seite gerendert werden soll, wenn das Projekt im grafischen Format gespeichert wird. Die Seitengröße wird geändert, damit das gerenderte Projekt auf eine Seite passt.

**Returns:**
boolean - ein Wert, der angibt, ob ein Projekt auf einer einzigen Seite gerendert werden soll, wenn das Projekt im grafischen Format gespeichert wird.
### getRollUpGanttBars() {#getRollUpGanttBars--}
```
public final boolean getRollUpGanttBars()
```


Gibt einen Wert zurück, der angibt, ob Teilaufgaben in der Zusammenfassungsaufgabenleiste markiert werden sollen. Für Teilaufgaben gibt das Rollup-Feld an, ob Informationen zu den Gantt-Balken der Teilaufgabe in die Zusammenfassungsaufgabenleiste übernommen werden. Für Zusammenfassungsaufgaben gibt das Rollup-Feld an, ob die Zusammenfassungsaufgabenleiste aggregierte Balken anzeigt. Das Rollup-Feld für Zusammenfassungsaufgaben muss auf Ja gesetzt sein, damit Teilaufgaben zu ihnen aggregiert werden.

--------------------

Gilt nur, wenn die Gantt-Diagrammansicht gerendert wird.

**Returns:**
boolean - ein Wert, der angibt, ob Teilaufgaben in der Zusammenfassungsaufgabenleiste markiert werden sollen.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


Ermittelt das Datum, ab dem das Rendern beginnen soll.

**Returns:**
java.util.Date - das Datum, ab dem gerendert werden soll.
### getTaskLinkDrawingCallback() {#getTaskLinkDrawingCallback--}
```
public final TaskLinkDrawingCallbackDelegate getTaskLinkDrawingCallback()
```


Ermittelt einen Callback, der verwendet werden kann, um einige Aspekte der Darstellung von Aufgabenverknüpfungen anzupassen.

Gilt nur, wenn die Gantt-Diagrammansicht gerendert wird.

**Returns:**
[TaskLinkDrawingCallbackDelegate](../../com.aspose.tasks/tasklinkdrawingcallbackdelegate) - a callback that can be used to customize some aspects of task links rendering.
### getTextStyles() {#getTextStyles--}
```
public final List<TextStyle> getTextStyles()
```


Ermittelt die Liste der Textstile, die während der Darstellung einer Projektansicht angewendet werden.

--------------------

Diese Stile überschreiben die mit GanttCharView.setTextStyles definierten Stile.

**Returns:**
java.util.List&lt;com.aspose.tasks.TextStyle&gt; - die Liste der Textstile, die während des Renderns einer Projektansicht angewendet werden.
### getTimescale() {#getTimescale--}
```
public final int getTimescale()
```


Ermittelt den `Timescale`([getTimescale()](../../com.aspose/tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose/tasks/saveoptions\#setTimescale-int-)) Wert, der verwendet wird, um zu steuern, wie die Zeitskala (falls vorhanden) gerendert wird, wenn das Projekt im grafischen Format gespeichert wird.

**Returns:**
int - der `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) Wert, der verwendet wird, um zu steuern, wie die Zeitskala (falls vorhanden) gerendert wird, wenn das Projekt im grafischen Format gespeichert wird.
### getTimescaleFitBehavior() {#getTimescaleFitBehavior--}
```
public final int getTimescaleFitBehavior()
```


Ermittelt ein Verhalten, das definiert, wie das rechte Ende der Zeitskala mit dem Seitenende ausgerichtet wird.

**Returns:**
int - ein Verhalten, das definiert, wie das rechte Ende der Zeitskala mit dem Seitenende ausgerichtet wird.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


Ermittelt einen Wert, der angibt, ob ein Farbverlaufspinsel beim Rendern des Gantt-Diagramms verwendet werden soll.

--------------------

Gilt nur, wenn die Gantt-Diagrammansicht gerendert wird.

**Returns:**
boolean - ein Wert, der angibt, ob ein Farbverlaufspinsel beim Rendern des Gantt-Diagramms verwendet werden soll.
### getView() {#getView--}
```
public final ProjectView getView()
```


Gibt eine Liste der Ansichtsspalten zurück, die gerendert werden sollen ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). Wenn nicht gesetzt, werden nur Aufgaben-IDs, Aufgabennamen, Start und Ende gerendert. Wenn sowohl View als auch `ViewSettings`([getViewSettings()](../../com.aspose.tasks/saveoptions\#getViewSettings--)/[setViewSettings(View)](../../com.aspose.tasks/saveoptions\#setViewSettings-View-)) Eigenschaften gesetzt sind, überschreiben die Spalten aus View die Spalten aus ViewSettings.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns to render ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)).
### getViewSettings() {#getViewSettings--}
```
public final View getViewSettings()
```


Gibt eine Ansicht (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) zurück, die gerendert werden soll. Mit dieser Option können Sie explizit festlegen, welche Ansicht in PDF-, HTML- oder Bildformate gespeichert werden soll. Ist diese Eigenschaft gesetzt, wird die [PresentationFormat](../../com.aspose.tasks/presentationformat)-Eigenschaft beim Speichern des Projekts ignoriert. Die Ansicht muss von einem der folgenden Bildschirme stammen ((`Aspose.Tasks.View.Screen`([View.getScreen()](../../com.aspose.tasks/view\#getScreen--)/[View.setScreen(int)](../../com.aspose.tasks/view\#setScreen-int-)))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage)

**Returns:**
[View](../../com.aspose.tasks/view) - a view (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) to render.
### isPortrait() {#isPortrait--}
```
public final boolean isPortrait()
```


Gibt einen Wert zurück, der angibt, ob die Seitenorientierung Hochformat ist; gibt false zurück, wenn die Seitenorientierung Querformat ist.

--------------------

Ist nicht anwendbar, wenn SaveOptions.getPageSize() == PageSize.DefinedInView. In diesem Fall wird [PageSettings.isPortrait()](../../com.aspose/tasks/pagesettings\#isPortrait--) verwendet. Ist nicht anwendbar, wenn [getCustomPageSize()](../../com.aspose/tasks/saveoptions\#getCustomPageSize--) gesetzt ist.

**Returns:**
boolean - ein Wert, der angibt, ob die Seitenorientierung Hochformat ist; gibt false zurück, wenn die Seitenorientierung Querformat ist.
### setBarStyles(List&lt;BarStyle&gt; value) {#setBarStyles-java.util.List-com.aspose.tasks.BarStyle--}
```
public final void setBarStyles(List<BarStyle> value)
```


Legt die Liste der Instanzen der Klasse [BarStyle](../../com.aspose/tasks/barstyle) fest, die in der Projektansicht erscheinen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.BarStyle&gt; | die Liste der Instanzen der Klasse [BarStyle](../../com.aspose/tasks/barstyle), die in der Projektansicht erscheinen. |

### setCustomPageSize(Dimension2D value) {#setCustomPageSize-java.awt.geom.Dimension2D-}
```
public final void setCustomPageSize(Dimension2D value)
```


Legt die benutzerdefinierte Seitengröße in Punkten fest (1 Punkt = 1/72 Zoll).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.awt.geom.Dimension2D | die benutzerdefinierte Seitengröße in Punkten (1 Punkt = 1/72 Zoll). |

### setDrawNonWorkingTime(boolean value) {#setDrawNonWorkingTime-boolean-}
```
public final void setDrawNonWorkingTime(boolean value)
```


Legt einen Wert fest, der angibt, ob Nichtarbeitszeit gezeichnet werden soll (Standardwert ist TRUE).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob Nichtarbeitszeit gezeichnet werden soll (Standardwert ist TRUE). |

### setEndDate(Date value) {#setEndDate-java.util.Date-}
```
public final void setEndDate(Date value)
```


Legt ein Datum fest, bis zu dem das Rendern abgeschlossen sein soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date | ein Datum, bis zu dem das Rendern abgeschlossen werden soll. |

### setFitContent(boolean value) {#setFitContent-boolean-}
```
public final void setFitContent(boolean value)
```


Legt einen Wert fest, der angibt, ob die Zeilenhöhe erhöht werden soll, um den Inhalt anzupassen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob die Zeilenhöhe erhöht werden soll, um den Inhalt anzupassen. |

### setGridlines(List&lt;Gridline&gt; value) {#setGridlines-java.util.List-com.aspose.tasks.Gridline--}
```
public final void setGridlines(List<Gridline> value)
```


Legt eine Liste von [Gridline](../../com.aspose/tasks/gridline) fest, die in der Projektansicht erscheinen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.Gridline&gt; | eine Liste von [Gridline](../../com.aspose/tasks/gridline), die in der Projektansicht erscheinen. |

### setLegendDrawingOptions(int value) {#setLegendDrawingOptions-int-}
```
public final void setLegendDrawingOptions(int value)
```


Legt einen Wert fest, der definiert, wie eine Legende gerendert wird. Standardwert ist LegendDrawingOptions.OnEveryPage.

Gilt nur, wenn die Gantt-Diagrammansicht gerendert wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | ein Wert, der definiert, wie eine Legende gerendert wird. |

### setLegendItems(PageLegendItem[] value) {#setLegendItems-com.aspose.tasks.PageLegendItem---}
```
public final void setLegendItems(PageLegendItem[] value)
```


Legt ein Array von PageLegendItem fest, das definiert, welche Balken in der Seitenlegende gerendert werden sollen. Wenn null, werden die Standardobjekte gerendert.

Gilt nur, wenn die Gantt-Diagrammansicht gerendert wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [PageLegendItem\[\]](../../com.aspose.tasks/pagelegenditem) | ein Array von PageLegendItem, das definiert, welche Balken in der Seitenlegende gerendert werden sollen. |

### setMarkCriticalTasks(boolean value) {#setMarkCriticalTasks-boolean-}
```
public final void setMarkCriticalTasks(boolean value)
```


Legt einen Wert fest, der angibt, ob kritische Aufgaben in roter Farbe angezeigt werden sollen (Standardwert ist FALSE).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob kritische Aufgaben in roter Farbe angezeigt werden sollen (Standardwert ist FALSE). |

### setNonWorkingTimeColor(Color value) {#setNonWorkingTimeColor-java.awt.Color-}
```
public final void setNonWorkingTimeColor(Color value)
```


Legt die Farbe für Nichtarbeitszeit fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.awt.Color | die Farbe für Nichtarbeitszeit. |

### setPageSize(int value) {#setPageSize-int-}
```
public final void setPageSize(int value)
```


Legt die Größe der zu rendernden Seite fest (Standardwert ist PageSize.A4).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | die Größe der zu rendernden Seite (Standardwert ist PageSize.A4). |

### setPortrait(boolean value) {#setPortrait-boolean-}
```
public final void setPortrait(boolean value)
```


Setzt einen Wert, der angibt, ob die Seitenorientierung Hochformat ist; gibt false zurück, wenn die Seitenorientierung Querformat ist.

--------------------

Ist nicht anwendbar, wenn SaveOptions.PageSize == Visualization.PageSize.DefinedInView. In diesem Fall wird [PageSettings.setPortrait(boolean)](../../com.aspose/tasks/pagesettings\#setPortrait-boolean-) verwendet. Ist nicht anwendbar, wenn [getCustomPageSize()](../../com.aspose/tasks/saveoptions\#getCustomPageSize--) gesetzt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob die Seitenorientierung Hochformat ist; gibt false zurück, wenn die Seitenorientierung Querformat ist. |

### setPresentationFormat(int value) {#setPresentationFormat-int-}
```
public final void setPresentationFormat(int value)
```


Legt das `PresentationFormat`([getPresentationFormat()](../../com.aspose/tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose/tasks/saveoptions\#setPresentationFormat-int-)) fest, in dem das Dokument gespeichert wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | int | das `PresentationFormat`([getPresentationFormat()](../../com.aspose/tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose/tasks/saveoptions\#setPresentationFormat-int-)), in dem das Dokument gespeichert wird. |

### setRenderToSinglePage(boolean value) {#setRenderToSinglePage-boolean-}
```
public final void setRenderToSinglePage(boolean value)
```


Legt einen Wert fest, der angibt, ob ein Projekt auf einer einzelnen Seite gerendert werden soll, wenn das Projekt im grafischen Format gespeichert wird. Die Seitengröße wird geändert, sodass das gerenderte Projekt auf eine Seite passt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob ein Projekt auf einer einzelnen Seite gerendert werden soll, wenn das Projekt im grafischen Format gespeichert wird. |

### setRollUpGanttBars(boolean value) {#setRollUpGanttBars-boolean-}
```
public final void setRollUpGanttBars(boolean value)
```


Legt einen Wert fest, der angibt, ob Unteraufgaben in der Balkenanzeige der Zusammenfassungsaufgabe markiert werden sollen. Für Unteraufgaben gibt das Feld Rollup an, ob Informationen zu den Gantt‑Balken der Unteraufgabe in den Balken der Zusammenfassungsaufgabe übernommen werden. Für Zusammenfassungsaufgaben gibt das Feld Rollup an, ob der Balken der Zusammenfassungsaufgabe aggregierte Balken anzeigt. Das Feld Rollup für Zusammenfassungsaufgaben muss auf Ja gesetzt sein, damit Unteraufgaben zu ihnen aggregiert werden können.

--------------------

Gilt nur, wenn die Gantt-Diagrammansicht gerendert wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob Unteraufgaben in der Balkenanzeige der Zusammenfassungsaufgabe markiert werden sollen. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


Legt das Datum fest, ab dem gerendert werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date | das Datum, ab dem das Rendern beginnen soll. |

### setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value) {#setTaskLinkDrawingCallback-com.aspose.tasks.TaskLinkDrawingCallbackDelegate-}
```
public final void setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value)
```


Legt einen Callback fest, der verwendet werden kann, um einige Aspekte der Darstellung von Aufgabenverknüpfungen anzupassen.

Gilt nur, wenn die Gantt-Diagrammansicht gerendert wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [TaskLinkDrawingCallbackDelegate](../../com.aspose.tasks/tasklinkdrawingcallbackdelegate) | ein Callback, der verwendet werden kann, um einige Aspekte der Darstellung von Aufgabenverknüpfungen anzupassen. |

### setTextStyles(List&lt;TextStyle&gt; value) {#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--}
```
public final void setTextStyles(List<TextStyle> value)
```


Legt die Liste der Textstile fest, die während der Darstellung einer Projektansicht angewendet werden.

--------------------

Diese Stile überschreiben die mit GanttCharView.setTextStyles definierten Stile.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.List&lt;com.aspose.tasks.TextStyle&gt; | die Liste der Textstile, die beim Rendern einer Projektansicht angewendet werden. |

### setTimescale(int value) {#setTimescale-int-}
```
public final void setTimescale(int value)
```


Legt den `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) Wert fest, der verwendet wird, um zu steuern, wie die Zeitskala (falls vorhanden) gerendert wird, wenn das Projekt im grafischen Format gespeichert wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | int | der `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) Wert, der verwendet wird, um zu steuern, wie die Zeitskala (falls vorhanden) gerendert wird, wenn das Projekt in ein grafisches Format gespeichert wird. |

### setTimescaleFitBehavior(int value) {#setTimescaleFitBehavior-int-}
```
public final void setTimescaleFitBehavior(int value)
```


Legt ein Verhalten fest, das definiert, wie das rechte Ende der Zeitskala mit dem Seitenende ausgerichtet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | ein Verhalten, das definiert, wie das rechte Ende der Zeitskala mit dem Seitenende ausgerichtet wird. |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


Legt einen Wert fest, der angibt, ob ein Farbverlaufspinsel beim Rendern des Gantt-Diagramms verwendet werden soll.

--------------------

Gilt nur, wenn die Gantt-Diagrammansicht gerendert wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob ein Farbverlaufspinsel beim Rendern des Gantt-Diagramms verwendet werden soll. |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


Legt eine Liste der Ansichtsspalten fest, die gerendert werden sollen ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). Wenn nicht festgelegt, werden nur Aufgaben‑IDs, Aufgabennamen, Start und Ende gerendert. Wenn sowohl View als auch `ViewSettings`([getViewSettings()](../../com.aspose.tasks/saveoptions\#getViewSettings--)/[setViewSettings(View)](../../com.aspose.tasks/saveoptions\#setViewSettings-View-)) Eigenschaften gesetzt sind, überschreiben die Spalten aus View die Spalten aus ViewSettings.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | eine Liste der Ansichtsspalten, die gerendert werden sollen ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |

### setViewSettings(View value) {#setViewSettings-com.aspose.tasks.View-}
```
public final void setViewSettings(View value)
```


Legt eine Ansicht (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) fest, die gerendert werden soll. Sie können diese Option verwenden, um explizit anzugeben, welche Ansicht in PDF-, HTML- oder Bildformate gespeichert werden soll. Ist diese Eigenschaft gesetzt, wird die [PresentationFormat](../../com.aspose.tasks/presentationformat)‑Eigenschaft beim Speichern des Projekts ignoriert. Die Ansicht muss von einem der folgenden Bildschirme stammen ((`Aspose.Tasks.View.Screen`([View.getScreen()](../../com.aspose.tasks/view\#getScreen--)/[View.setScreen(int)](../../com.aspose.tasks/view\#setScreen-int-)))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [View](../../com.aspose.tasks/view) | eine Ansicht (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) zum Rendern. |

