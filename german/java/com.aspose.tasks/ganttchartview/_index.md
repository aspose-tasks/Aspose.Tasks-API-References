---
title: "GanttChartView"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt eine GanttChart‑Ansicht dar."
type: docs
weight: 112
url: /de/java/com.aspose.tasks/ganttchartview/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.View](../../com.aspose.tasks/view)

**All Implemented Interfaces:**
com.aspose.tasks.ITimescaledView
```
public class GanttChartView extends View implements ITimescaledView
```

Stellt eine GanttChart‑Ansicht dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [GanttChartView()](#GanttChartView--) | Initialisiert eine neue Instanz der Klasse [GanttChartView](../../com.aspose.tasks/ganttchartview). |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getAutoFilters()](#getAutoFilters--) | Ruft eine Liste von Auto-Filtern einer Gantt Chart-Ansicht ab. |
| [getBarRounding()](#getBarRounding--) | Ruft einen Wert ab, der angibt, ob die Balken auf den nächsten Tag gerundet werden. |
| [getBarSize()](#getBarSize--) | Ermittelt die Höhe, in Punkten, der Gantt-Balken im Gantt-Diagramm. |
| [getBarStyles()](#getBarStyles--) | Ermittelt eine Liste der übergeordneten (gemeinsamen) Balkenstile der Gantt-Diagrammansicht. |
| [getBottomTimescaleTier()](#getBottomTimescaleTier--) | Liefert die Einstellungen der unteren Zeitskala-Ebene der Ansicht. |
| [getCustomBarStyles()](#getCustomBarStyles--) | Ermittelt eine Liste benutzerdefinierter, aufgabenbezogener Balkenstile der Gantt-Diagrammansicht. |
| [getGridlines()](#getGridlines--) | Ermittelt eine Liste von `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) der Gantt-Diagrammansicht. |
| [getHideRollupBarsWhenSummaryExpanded()](#getHideRollupBarsWhenSummaryExpanded--) | Ermittelt einen Wert, der angibt, ob Rollup-Balken beim Erweitern der Zusammenfassungsaufgabe ausgeblendet werden. |
| [getMiddleTimescaleTier()](#getMiddleTimescaleTier--) | Liefert die Einstellungen der mittleren Zeitskala-Ebene der Ansicht. |
| [getNonWorkingTimeColor()](#getNonWorkingTimeColor--) | Ermittelt die Farbe für Nichtarbeitszeit. |
| [getProgressLines()](#getProgressLines--) | Ermittelt Fortschrittslinien für die Gantt-Diagrammansicht. |
| [getRollUpGanttBars()](#getRollUpGanttBars--) | Ermittelt einen Wert, der angibt, ob Balken im Gantt-Diagramm zusammengefasst werden müssen. |
| [getShowBarSplits()](#getShowBarSplits--) | Ermittelt einen Wert, der angibt, ob Aufgabenteilungen im Gantt-Diagramm angezeigt werden müssen. |
| [getShowDrawings()](#getShowDrawings--) | Ermittelt einen Wert, der angibt, ob Zeichnungen im Gantt-Diagramm angezeigt werden müssen. |
| [getTableTextStyles()](#getTableTextStyles--) | Ermittelt eine Liste von Tabellentextstilen der Gantt-Diagrammansicht. |
| [getTextStyles()](#getTextStyles--) | Ermittelt eine Liste von [TextStyle](../../com.aspose.tasks/textstyle) der Gantt-Diagrammansicht. |
| [getTimescaleSizePercentage()](#getTimescaleSizePercentage--) | \{@inheritDoc\} |
| [getTopTimescaleTier()](#getTopTimescaleTier--) | Liefert die Einstellungen der oberen Zeitskala-Ebene der Ansicht. |
| [setBarRounding(boolean value)](#setBarRounding-boolean-) | Legt einen Wert fest, der angibt, ob die Balken auf den nächsten Tag gerundet werden. |
| [setBarSize(int value)](#setBarSize-int-) | Legt die Höhe der Gantt-Balken im Gantt-Diagramm in Punkten fest. |
| [setBottomTimescaleTier(TimescaleTier value)](#setBottomTimescaleTier-com.aspose.tasks.TimescaleTier-) | Setzt die Einstellungen der unteren Zeitskala-Ebene der Ansicht. |
| [setGridlines(List&lt;Gridlines&gt; value)](#setGridlines-java.util.List-com.aspose.tasks.Gridlines--) | Legt eine Liste von `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) der Gantt-Diagrammansicht fest. |
| [setHideRollupBarsWhenSummaryExpanded(boolean value)](#setHideRollupBarsWhenSummaryExpanded-boolean-) | Legt einen Wert fest, der angibt, ob Rollup-Balken beim Erweitern der Zusammenfassungsaufgabe ausgeblendet werden. |
| [setMiddleTimescaleTier(TimescaleTier value)](#setMiddleTimescaleTier-com.aspose.tasks.TimescaleTier-) | Legt die Einstellungen der mittleren Zeitskala‑Stufe der Ansicht fest. |
| [setNonWorkingTimeColor(Color value)](#setNonWorkingTimeColor-java.awt.Color-) | Legt die Farbe für Nichtarbeitszeit fest. |
| [setProgressLines(ProgressLines value)](#setProgressLines-com.aspose.tasks.ProgressLines-) | Legt Fortschrittslinien für die Gantt-Diagrammansicht fest. |
| [setRollUpGanttBars(boolean value)](#setRollUpGanttBars-boolean-) | Legt einen Wert fest, der angibt, ob Balken im Gantt-Diagramm zusammengefasst werden müssen. |
| [setShowBarSplits(boolean value)](#setShowBarSplits-boolean-) | Legt einen Wert fest, der angibt, ob Aufgabenteilungen im Gantt-Diagramm angezeigt werden müssen. |
| [setShowDrawings(boolean value)](#setShowDrawings-boolean-) | Legt einen Wert fest, der angibt, ob Zeichnungen im Gantt-Diagramm angezeigt werden müssen. |
| [setTextStyles(List&lt;TextStyle&gt; value)](#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--) | Legt eine Liste von [TextStyle](../../com.aspose.tasks/textstyle) der Gantt-Diagrammansicht fest. |
| [setTimescaleSizePercentage(int value)](#setTimescaleSizePercentage-int-) | \{@inheritDoc\} |
| [setTopTimescaleTier(TimescaleTier value)](#setTopTimescaleTier-com.aspose.tasks.TimescaleTier-) | Legt die Einstellungen der oberen Zeitskala‑Stufe der Ansicht fest. |
### GanttChartView() {#GanttChartView--}
```
public GanttChartView()
```


Initialisiert eine neue Instanz der Klasse [GanttChartView](../../com.aspose.tasks/ganttchartview).

### getAutoFilters() {#getAutoFilters--}
```
public final FilterCollection getAutoFilters()
```


Ruft eine Liste von Auto-Filtern einer Gantt Chart-Ansicht ab.

**Returns:**
[FilterCollection](../../com.aspose.tasks/filtercollection) - a list of auto filters of a Gantt Chart view.
### getBarRounding() {#getBarRounding--}
```
public final boolean getBarRounding()
```


Ermittelt einen Wert, der angibt, ob die Balken auf den nächsten Tag gerundet werden. Der Standardwert ist True.

**Returns:**
boolean - ein Wert, der angibt, ob die Balken auf den nächsten Tag gerundet werden.
### getBarSize() {#getBarSize--}
```
public final int getBarSize()
```


Ermittelt die Höhe, in Punkten, der Gantt-Balken im Gantt-Diagramm.

**Returns:**
int - die Höhe, in Punkten, der Gantt-Balken im Gantt-Diagramm.
### getBarStyles() {#getBarStyles--}
```
public final List<GanttBarStyle> getBarStyles()
```


Ruft eine Liste der übergeordneten (gemeinsamen) Balkenstile der Gantt-Diagrammansicht ab. [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.GanttBarStyle&gt; - eine Liste der übergeordneten (gemeinsamen) Balkenstile der Gantt-Diagrammansicht.
### getBottomTimescaleTier() {#getBottomTimescaleTier--}
```
public final TimescaleTier getBottomTimescaleTier()
```


Liest die Einstellungen der unteren Zeitskala‑Stufe der Ansicht. [TimescaleTier](../../com.aspose.tasks/timescaletier)

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's bottom timescale tier.
### getCustomBarStyles() {#getCustomBarStyles--}
```
public final List<GanttBarStyle> getCustomBarStyles()
```


Ruft eine Liste benutzerdefinierter, aufgabenbezogener Balkenstile der Gantt-Diagrammansicht ab. [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.GanttBarStyle&gt; - eine Liste benutzerdefinierter, aufgabenbezogener Balkenstile der Gantt-Diagrammansicht.
### getGridlines() {#getGridlines--}
```
public final List<Gridlines> getGridlines()
```


Ermittelt eine Liste von `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) der Gantt-Diagrammansicht.

**Returns:**
java.util.List&lt;com.aspose.tasks.Gridlines&gt; - eine Liste von `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) der Gantt-Diagrammansicht.
### getHideRollupBarsWhenSummaryExpanded() {#getHideRollupBarsWhenSummaryExpanded--}
```
public final boolean getHideRollupBarsWhenSummaryExpanded()
```


Ermittelt einen Wert, der angibt, ob Rollup-Balken beim Erweitern der Zusammenfassungsaufgabe ausgeblendet werden.

**Returns:**
boolean - ein Wert, der angibt, ob Rollup-Balken beim Erweitern einer Zusammenfassungsaufgabe ausgeblendet werden.
### getMiddleTimescaleTier() {#getMiddleTimescaleTier--}
```
public final TimescaleTier getMiddleTimescaleTier()
```


Liest die Einstellungen der mittleren Zeitskala‑Stufe der Ansicht. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's middle timescale tier.
### getNonWorkingTimeColor() {#getNonWorkingTimeColor--}
```
public final Color getNonWorkingTimeColor()
```


Ermittelt die Farbe für Nichtarbeitszeit.

**Returns:**
java.awt.Color - Farbe für Nichtarbeitszeit.
### getProgressLines() {#getProgressLines--}
```
public final ProgressLines getProgressLines()
```


Ruft Fortschrittslinien für die Gantt-Diagrammansicht ab. `ProgressLines`([getProgressLines()](../../com.aspose.tasks/ganttchartview\#getProgressLines--)/[setProgressLines(ProgressLines)](../../com.aspose.tasks/ganttchartview\#setProgressLines-ProgressLines-)).

**Returns:**
[ProgressLines](../../com.aspose.tasks/progresslines) - progress lines for the Gantt Chart view.
### getRollUpGanttBars() {#getRollUpGanttBars--}
```
public final boolean getRollUpGanttBars()
```


Ermittelt einen Wert, der angibt, ob Balken im Gantt-Diagramm zusammengefasst werden müssen.

**Returns:**
boolean - ein Wert, der angibt, ob Balken im Gantt-Diagramm zusammengefasst werden müssen.
### getShowBarSplits() {#getShowBarSplits--}
```
public final boolean getShowBarSplits()
```


Ermittelt einen Wert, der angibt, ob Aufgabenteilungen im Gantt-Diagramm angezeigt werden müssen.

**Returns:**
boolean - ein Wert, der angibt, ob Aufgabenteilungen im Gantt-Diagramm angezeigt werden sollen.
### getShowDrawings() {#getShowDrawings--}
```
public final boolean getShowDrawings()
```


Ermittelt einen Wert, der angibt, ob Zeichnungen im Gantt-Diagramm angezeigt werden müssen.

**Returns:**
boolean - ein Wert, der angibt, ob Zeichnungen im Gantt-Diagramm angezeigt werden sollen.
### getTableTextStyles() {#getTableTextStyles--}
```
public final List<TableTextStyle> getTableTextStyles()
```


Ruft eine Liste von Tabellentextstilen der Gantt-Diagrammansicht ab. [TableTextStyle](../../com.aspose.tasks/tabletextstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.TableTextStyle&gt; - eine Liste von Tabellentextstilen der Gantt-Diagrammansicht.
### getTextStyles() {#getTextStyles--}
```
public final List<TextStyle> getTextStyles()
```


Ermittelt eine Liste von [TextStyle](../../com.aspose.tasks/textstyle) der Gantt-Diagrammansicht.

**Returns:**
java.util.List&lt;com.aspose.tasks.TextStyle&gt; - eine Liste von [TextStyle](../../com.aspose.tasks/textstyle) der Gantt-Diagrammansicht.
### getTimescaleSizePercentage() {#getTimescaleSizePercentage--}
```
public final int getTimescaleSizePercentage()
```


Liest einen Prozentsatz, um den Abstand zwischen Einheiten auf der Zeitskala‑Stufe zu verkleinern oder zu vergrößern.

**Returns:**
int - \{@inheritDoc\}
### getTopTimescaleTier() {#getTopTimescaleTier--}
```
public final TimescaleTier getTopTimescaleTier()
```


Liest die Einstellungen der oberen Zeitskala‑Stufe der Ansicht. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's top timescale tier.
### setBarRounding(boolean value) {#setBarRounding-boolean-}
```
public final void setBarRounding(boolean value)
```


Legt einen Wert fest, der angibt, ob die Balken auf den nächsten Tag gerundet werden. Der Standardwert ist True.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob die Balken auf den nächsten Tag gerundet werden. |

### setBarSize(int value) {#setBarSize-int-}
```
public final void setBarSize(int value)
```


Legt die Höhe der Gantt-Balken im Gantt-Diagramm in Punkten fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | die Höhe der Gantt-Balken im Gantt-Diagramm, angegeben in Punkten. |

### setBottomTimescaleTier(TimescaleTier value) {#setBottomTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setBottomTimescaleTier(TimescaleTier value)
```


Legt die Einstellungen der unteren Zeitskala‑Stufe der Ansicht fest. [TimescaleTier](../../com.aspose.tasks/timescaletier)

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | Einstellungen der unteren Zeitskala‑Stufe der Ansicht. |

### setGridlines(List&lt;Gridlines&gt; value) {#setGridlines-java.util.List-com.aspose.tasks.Gridlines--}
```
public final void setGridlines(List<Gridlines> value)
```


Legt eine Liste von `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) der Gantt-Diagrammansicht fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.Gridlines&gt; | eine Liste von `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) der Gantt-Diagrammansicht. |

### setHideRollupBarsWhenSummaryExpanded(boolean value) {#setHideRollupBarsWhenSummaryExpanded-boolean-}
```
public final void setHideRollupBarsWhenSummaryExpanded(boolean value)
```


Legt einen Wert fest, der angibt, ob Rollup-Balken beim Erweitern der Zusammenfassungsaufgabe ausgeblendet werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob Rollup-Balken beim Erweitern einer Zusammenfassungsaufgabe ausgeblendet werden. |

### setMiddleTimescaleTier(TimescaleTier value) {#setMiddleTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setMiddleTimescaleTier(TimescaleTier value)
```


Legt die Einstellungen der mittleren Zeitskala‑Stufe der Ansicht fest. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | Einstellungen der mittleren Zeitskala‑Stufe der Ansicht. |

### setNonWorkingTimeColor(Color value) {#setNonWorkingTimeColor-java.awt.Color-}
```
public final void setNonWorkingTimeColor(Color value)
```


Legt die Farbe für Nichtarbeitszeit fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.awt.Color | Farbe für Nichtarbeitszeit. |

### setProgressLines(ProgressLines value) {#setProgressLines-com.aspose.tasks.ProgressLines-}
```
public final void setProgressLines(ProgressLines value)
```


Legt Fortschrittslinien für die Gantt-Diagrammansicht fest. `ProgressLines`([getProgressLines()](../../com.aspose.tasks/ganttchartview\#getProgressLines--)/[setProgressLines(ProgressLines)](../../com.aspose.tasks/ganttchartview\#setProgressLines-ProgressLines-)).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [ProgressLines](../../com.aspose.tasks/progresslines) | Fortschrittslinien für die Gantt-Diagrammansicht. |

### setRollUpGanttBars(boolean value) {#setRollUpGanttBars-boolean-}
```
public final void setRollUpGanttBars(boolean value)
```


Legt einen Wert fest, der angibt, ob Balken im Gantt-Diagramm zusammengefasst werden müssen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob Balken im Gantt-Diagramm zusammengefasst werden müssen. |

### setShowBarSplits(boolean value) {#setShowBarSplits-boolean-}
```
public final void setShowBarSplits(boolean value)
```


Legt einen Wert fest, der angibt, ob Aufgabenteilungen im Gantt-Diagramm angezeigt werden müssen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob Aufgabenteilungen im Gantt-Diagramm angezeigt werden sollen. |

### setShowDrawings(boolean value) {#setShowDrawings-boolean-}
```
public final void setShowDrawings(boolean value)
```


Legt einen Wert fest, der angibt, ob Zeichnungen im Gantt-Diagramm angezeigt werden müssen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob Zeichnungen im Gantt-Diagramm angezeigt werden sollen. |

### setTextStyles(List&lt;TextStyle&gt; value) {#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--}
```
public final void setTextStyles(List<TextStyle> value)
```


Legt eine Liste von [TextStyle](../../com.aspose.tasks/textstyle) der Gantt-Diagrammansicht fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.TextStyle&gt; | eine Liste von [TextStyle](../../com.aspose.tasks/textstyle) der Gantt-Diagramm-Ansicht. |

### setTimescaleSizePercentage(int value) {#setTimescaleSizePercentage-int-}
```
public final void setTimescaleSizePercentage(int value)
```


Legt einen Prozentsatz fest, um den Abstand zwischen Einheiten auf der Zeitskala‑Stufe zu verkleinern oder zu vergrößern.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | \{@inheritDoc\} |

### setTopTimescaleTier(TimescaleTier value) {#setTopTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setTopTimescaleTier(TimescaleTier value)
```


Legt die Einstellungen der oberen Zeitskala‑Stufe der Ansicht fest. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | Einstellungen der oberen Zeitskala‑Stufe der Ansicht. |

