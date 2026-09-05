---
title: "GanttChartView"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een GanttChart‑weergave voor."
type: docs
weight: 112
url: /nl/java/com.aspose.tasks/ganttchartview/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.View](../../com.aspose.tasks/view)

**All Implemented Interfaces:**
com.aspose.tasks.ITimescaledView
```
public class GanttChartView extends View implements ITimescaledView
```

Stelt een GanttChart‑weergave voor.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [GanttChartView()](#GanttChartView--) | Initialiseert een nieuw exemplaar van de klasse [GanttChartView](../../com.aspose.tasks/ganttchartview). |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getAutoFilters()](#getAutoFilters--) | Haalt een lijst op van automatische filters van een Gantt Chart-weergave. |
| [getBarRounding()](#getBarRounding--) | Haalt een waarde op die aangeeft of de balken naar de dichtstbijzijnde dag worden afgerond. |
| [getBarSize()](#getBarSize--) | Haalt de hoogte, in punten, van de Gantt-balken in de Gantt Chart op. |
| [getBarStyles()](#getBarStyles--) | Haalt een lijst op van bovenliggende (gemeenschappelijke) balkstijlen van de Gantt Chart-weergave. |
| [getBottomTimescaleTier()](#getBottomTimescaleTier--) | Haalt de instellingen van de onderste tijdschaallaag van de weergave op. |
| [getCustomBarStyles()](#getCustomBarStyles--) | Haalt een lijst op van aangepaste taak‑specifieke balkstijlen van de Gantt Chart-weergave. |
| [getGridlines()](#getGridlines--) | Haalt een lijst op van `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) van de Gantt Chart-weergave. |
| [getHideRollupBarsWhenSummaryExpanded()](#getHideRollupBarsWhenSummaryExpanded--) | Haalt een waarde op die aangeeft of roll‑up balken verborgen worden bij het uitvouwen van een samenvattende taak. |
| [getMiddleTimescaleTier()](#getMiddleTimescaleTier--) | Haalt de instellingen van de middelste tijdschaallaag van de weergave op. |
| [getNonWorkingTimeColor()](#getNonWorkingTimeColor--) | Haalt de kleur voor niet‑werkelijke tijd op. |
| [getProgressLines()](#getProgressLines--) | Haalt voortgangslijnen op voor de Gantt Chart-weergave. |
| [getRollUpGanttBars()](#getRollUpGanttBars--) | Haalt een waarde op die aangeeft of balken op de Gantt Chart moeten worden samengevoegd. |
| [getShowBarSplits()](#getShowBarSplits--) | Haalt een waarde op die aangeeft of taak‑splitsingen op de Gantt Chart moeten worden weergegeven. |
| [getShowDrawings()](#getShowDrawings--) | Haalt een waarde op die aangeeft of tekeningen op de Gantt Chart moeten worden weergegeven. |
| [getTableTextStyles()](#getTableTextStyles--) | Haalt een lijst op van tabeltekststijlen van de Gantt Chart-weergave. |
| [getTextStyles()](#getTextStyles--) | Haalt een lijst op van [TextStyle](../../com.aspose.tasks/textstyle) van de Gantt Chart-weergave. |
| [getTimescaleSizePercentage()](#getTimescaleSizePercentage--) | \{@inheritDoc\} |
| [getTopTimescaleTier()](#getTopTimescaleTier--) | Haalt de instellingen van de bovenste tijdschaallaag van de weergave op. |
| [setBarRounding(boolean value)](#setBarRounding-boolean-) | Stelt een waarde in die aangeeft of de balken naar de dichtstbijzijnde dag worden afgerond. |
| [setBarSize(int value)](#setBarSize-int-) | Stelt de hoogte, in punten, van de Gantt-balken in de Gantt Chart in. |
| [setBottomTimescaleTier(TimescaleTier value)](#setBottomTimescaleTier-com.aspose.tasks.TimescaleTier-) | Stelt de instellingen van de onderste tijdschaallaag van de weergave in. |
| [setGridlines(List&lt;Gridlines&gt; value)](#setGridlines-java.util.List-com.aspose.tasks.Gridlines--) | Stelt een lijst in van `Gridlines`([getGridlines()](../../com.aspose/tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose/tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) van de Gantt-diagramweergave. |
| [setHideRollupBarsWhenSummaryExpanded(boolean value)](#setHideRollupBarsWhenSummaryExpanded-boolean-) | Stelt een waarde in die aangeeft of rollup-balken verborgen worden bij het uitvouwen van een samenvattende taak. |
| [setMiddleTimescaleTier(TimescaleTier value)](#setMiddleTimescaleTier-com.aspose.tasks.TimescaleTier-) | Stelt de instellingen van de middelste tijdschaallaag van de weergave in. |
| [setNonWorkingTimeColor(Color value)](#setNonWorkingTimeColor-java.awt.Color-) | Stelt de kleur voor niet-werkende tijd in. |
| [setProgressLines(ProgressLines value)](#setProgressLines-com.aspose.tasks.ProgressLines-) | Stelt voortgangslijnen in voor de Gantt-diagramweergave. |
| [setRollUpGanttBars(boolean value)](#setRollUpGanttBars-boolean-) | Stelt een waarde in die aangeeft of balken op de Gantt-diagram moeten worden samengevoegd. |
| [setShowBarSplits(boolean value)](#setShowBarSplits-boolean-) | Stelt een waarde in die aangeeft of taakonderbrekingen op de Gantt-diagram moeten worden weergegeven. |
| [setShowDrawings(boolean value)](#setShowDrawings-boolean-) | Stelt een waarde in die aangeeft of tekeningen op de Gantt-diagram moeten worden weergegeven. |
| [setTextStyles(List&lt;TextStyle&gt; value)](#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--) | Stelt een lijst in van [TextStyle](../../com.aspose.tasks/textstyle) van de Gantt-diagramweergave. |
| [setTimescaleSizePercentage(int value)](#setTimescaleSizePercentage-int-) | \{@inheritDoc\} |
| [setTopTimescaleTier(TimescaleTier value)](#setTopTimescaleTier-com.aspose.tasks.TimescaleTier-) | Stelt de instellingen van de bovenste tijdschaallaag van de weergave in. |
### GanttChartView() {#GanttChartView--}
```
public GanttChartView()
```


Initialiseert een nieuw exemplaar van de klasse [GanttChartView](../../com.aspose.tasks/ganttchartview).

### getAutoFilters() {#getAutoFilters--}
```
public final FilterCollection getAutoFilters()
```


Haalt een lijst op van automatische filters van een Gantt Chart-weergave.

**Returns:**
[FilterCollection](../../com.aspose.tasks/filtercollection) - a list of auto filters of a Gantt Chart view.
### getBarRounding() {#getBarRounding--}
```
public final boolean getBarRounding()
```


Haalt een waarde op die aangeeft of de balken afronden op de dichtstbijzijnde dag. De standaardwaarde is True.

**Returns:**
boolean - een waarde die aangeeft of de balken afronden op de dichtstbijzijnde dag.
### getBarSize() {#getBarSize--}
```
public final int getBarSize()
```


Haalt de hoogte, in punten, van de Gantt-balken in de Gantt Chart op.

**Returns:**
int - de hoogte, in punten, van de Gantt-balken in de Gantt-diagram.
### getBarStyles() {#getBarStyles--}
```
public final List<GanttBarStyle> getBarStyles()
```


Haalt een lijst op van bovenliggende (gemeenschappelijke) balkstijlen van de Gantt-diagramweergave. [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.GanttBarStyle&gt; - een lijst van bovenliggende (gemeenschappelijke) balkstijlen van de Gantt-diagramweergave.
### getBottomTimescaleTier() {#getBottomTimescaleTier--}
```
public final TimescaleTier getBottomTimescaleTier()
```


Haalt de instellingen van de onderste tijdschaallaag van de weergave op. [TimescaleTier](../../com.aspose.tasks/timescaletier)

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's bottom timescale tier.
### getCustomBarStyles() {#getCustomBarStyles--}
```
public final List<GanttBarStyle> getCustomBarStyles()
```


Haalt een lijst op van aangepaste taak-specifieke balkstijlen van de Gantt-diagramweergave. [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.GanttBarStyle&gt; - een lijst van aangepaste taak-specifieke balkstijlen van de Gantt-diagramweergave.
### getGridlines() {#getGridlines--}
```
public final List<Gridlines> getGridlines()
```


Haalt een lijst op van `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) van de Gantt Chart-weergave.

**Returns:**
java.util.List&lt;com.aspose.tasks.Gridlines&gt; - een lijst van `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) van de Gantt-diagramweergave.
### getHideRollupBarsWhenSummaryExpanded() {#getHideRollupBarsWhenSummaryExpanded--}
```
public final boolean getHideRollupBarsWhenSummaryExpanded()
```


Haalt een waarde op die aangeeft of roll‑up balken verborgen worden bij het uitvouwen van een samenvattende taak.

**Returns:**
boolean - een waarde die aangeeft of rollup-balken verborgen worden bij het uitvouwen van een samenvattende taak.
### getMiddleTimescaleTier() {#getMiddleTimescaleTier--}
```
public final TimescaleTier getMiddleTimescaleTier()
```


Haalt de instellingen van de middelste tijdschaallaag van de weergave op. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's middle timescale tier.
### getNonWorkingTimeColor() {#getNonWorkingTimeColor--}
```
public final Color getNonWorkingTimeColor()
```


Haalt de kleur voor niet‑werkelijke tijd op.

**Returns:**
java.awt.Color - kleur voor niet-werkende tijd.
### getProgressLines() {#getProgressLines--}
```
public final ProgressLines getProgressLines()
```


Haalt voortgangslijnen op voor de Gantt-diagramweergave. `ProgressLines`([getProgressLines()](../../com.aspose.tasks/ganttchartview\#getProgressLines--)/[setProgressLines(ProgressLines)](../../com.aspose.tasks/ganttchartview\#setProgressLines-ProgressLines-)).

**Returns:**
[ProgressLines](../../com.aspose.tasks/progresslines) - progress lines for the Gantt Chart view.
### getRollUpGanttBars() {#getRollUpGanttBars--}
```
public final boolean getRollUpGanttBars()
```


Haalt een waarde op die aangeeft of balken op de Gantt Chart moeten worden samengevoegd.

**Returns:**
boolean - een waarde die aangeeft of balken op de Gantt-diagram moeten worden samengevoegd.
### getShowBarSplits() {#getShowBarSplits--}
```
public final boolean getShowBarSplits()
```


Haalt een waarde op die aangeeft of taak‑splitsingen op de Gantt Chart moeten worden weergegeven.

**Returns:**
boolean - een waarde die aangeeft of taakonderbrekingen op de Gantt-diagram moeten worden weergegeven.
### getShowDrawings() {#getShowDrawings--}
```
public final boolean getShowDrawings()
```


Haalt een waarde op die aangeeft of tekeningen op de Gantt Chart moeten worden weergegeven.

**Returns:**
boolean - een waarde die aangeeft of tekeningen op de Gantt-diagram moeten worden weergegeven.
### getTableTextStyles() {#getTableTextStyles--}
```
public final List<TableTextStyle> getTableTextStyles()
```


Haalt een lijst op van tabeltekststijlen van de Gantt-diagramweergave. [TableTextStyle](../../com.aspose.tasks/tabletextstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.TableTextStyle&gt; - een lijst van tabeltekststijlen van de Gantt-diagramweergave.
### getTextStyles() {#getTextStyles--}
```
public final List<TextStyle> getTextStyles()
```


Haalt een lijst op van [TextStyle](../../com.aspose.tasks/textstyle) van de Gantt Chart-weergave.

**Returns:**
java.util.List&lt;com.aspose.tasks.TextStyle&gt; - een lijst van [TextStyle](../../com.aspose.tasks/textstyle) van de Gantt-diagramweergave.
### getTimescaleSizePercentage() {#getTimescaleSizePercentage--}
```
public final int getTimescaleSizePercentage()
```


Haalt een percentage op om de afstand tussen eenheden op de tijdschaallaag te verkleinen of te vergroten.

**Returns:**
int - \{@inheritDoc\}
### getTopTimescaleTier() {#getTopTimescaleTier--}
```
public final TimescaleTier getTopTimescaleTier()
```


Haalt de instellingen van de bovenste tijdschaallaag van de weergave op. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's top timescale tier.
### setBarRounding(boolean value) {#setBarRounding-boolean-}
```
public final void setBarRounding(boolean value)
```


Stelt een waarde in die aangeeft of de balken naar de dichtstbijzijnde dag worden afgerond. De standaardwaarde is True.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of de balken naar de dichtstbijzijnde dag worden afgerond. |

### setBarSize(int value) {#setBarSize-int-}
```
public final void setBarSize(int value)
```


Stelt de hoogte, in punten, van de Gantt-balken in de Gantt Chart in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | de hoogte, in punten, van de Gantt-balken in het Gantt-diagram. |

### setBottomTimescaleTier(TimescaleTier value) {#setBottomTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setBottomTimescaleTier(TimescaleTier value)
```


Stelt de instellingen van de onderste tijdschaallaag van de weergave in. [TimescaleTier](../../com.aspose.tasks/timescaletier)

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | instellingen van de onderste tijdschaallaag van de weergave. |

### setGridlines(List&lt;Gridlines&gt; value) {#setGridlines-java.util.List-com.aspose.tasks.Gridlines--}
```
public final void setGridlines(List<Gridlines> value)
```


Stelt een lijst in van `Gridlines`([getGridlines()](../../com.aspose/tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose/tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) van de Gantt-diagramweergave.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.Gridlines&gt; | een lijst van `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) van de Gantt-diagramweergave. |

### setHideRollupBarsWhenSummaryExpanded(boolean value) {#setHideRollupBarsWhenSummaryExpanded-boolean-}
```
public final void setHideRollupBarsWhenSummaryExpanded(boolean value)
```


Stelt een waarde in die aangeeft of rollup-balken verborgen worden bij het uitvouwen van een samenvattende taak.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of roll-up balken worden verborgen bij het uitvouwen van de samenvattende taak. |

### setMiddleTimescaleTier(TimescaleTier value) {#setMiddleTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setMiddleTimescaleTier(TimescaleTier value)
```


Stelt de instellingen van de middelste tijdschaallaag van de weergave in. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | instellingen van de middelste tijdschaallaag van de weergave. |

### setNonWorkingTimeColor(Color value) {#setNonWorkingTimeColor-java.awt.Color-}
```
public final void setNonWorkingTimeColor(Color value)
```


Stelt de kleur voor niet-werkende tijd in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.awt.Color | kleur voor niet-werkelijke tijd. |

### setProgressLines(ProgressLines value) {#setProgressLines-com.aspose.tasks.ProgressLines-}
```
public final void setProgressLines(ProgressLines value)
```


Stelt voortgangslijnen in voor de Gantt-diagramweergave. `ProgressLines`([getProgressLines()](../../com.aspose.tasks/ganttchartview\#getProgressLines--)/[setProgressLines(ProgressLines)](../../com.aspose.tasks/ganttchartview\#setProgressLines-ProgressLines-)).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [ProgressLines](../../com.aspose.tasks/progresslines) | voortgangslijnen voor de Gantt-diagramweergave. |

### setRollUpGanttBars(boolean value) {#setRollUpGanttBars-boolean-}
```
public final void setRollUpGanttBars(boolean value)
```


Stelt een waarde in die aangeeft of balken op de Gantt-diagram moeten worden samengevoegd.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of balken op het Gantt-diagram moeten worden opgerold. |

### setShowBarSplits(boolean value) {#setShowBarSplits-boolean-}
```
public final void setShowBarSplits(boolean value)
```


Stelt een waarde in die aangeeft of taakonderbrekingen op de Gantt-diagram moeten worden weergegeven.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of taakonderbrekingen op het Gantt-diagram moeten worden weergegeven. |

### setShowDrawings(boolean value) {#setShowDrawings-boolean-}
```
public final void setShowDrawings(boolean value)
```


Stelt een waarde in die aangeeft of tekeningen op de Gantt-diagram moeten worden weergegeven.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of tekeningen op het Gantt-diagram moeten worden weergegeven. |

### setTextStyles(List&lt;TextStyle&gt; value) {#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--}
```
public final void setTextStyles(List<TextStyle> value)
```


Stelt een lijst in van [TextStyle](../../com.aspose.tasks/textstyle) van de Gantt-diagramweergave.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.TextStyle&gt; | een lijst van [TextStyle](../../com.aspose.tasks/textstyle) van de Gantt-diagramweergave. |

### setTimescaleSizePercentage(int value) {#setTimescaleSizePercentage-int-}
```
public final void setTimescaleSizePercentage(int value)
```


Stelt een percentage in om de afstand tussen eenheden op de tijdschaallaag te verkleinen of te vergroten.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | \{@inheritDoc\} |

### setTopTimescaleTier(TimescaleTier value) {#setTopTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setTopTimescaleTier(TimescaleTier value)
```


Stelt de instellingen van de bovenste tijdschaallaag van de weergave in. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | instellingen van de bovenste tijdschaallaag van de weergave. |

