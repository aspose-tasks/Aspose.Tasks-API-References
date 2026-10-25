---
title: "GanttChartView"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar en GanttChart-vy."
type: docs
weight: 112
url: /sv/java/com.aspose.tasks/ganttchartview/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.View](../../com.aspose.tasks/view)

**All Implemented Interfaces:**
com.aspose.tasks.ITimescaledView
```
public class GanttChartView extends View implements ITimescaledView
```

Representerar en GanttChart-vy.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [GanttChartView()](#GanttChartView--) | Initierar en ny instans av klassen [GanttChartView](../../com.aspose.tasks/ganttchartview). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getAutoFilters()](#getAutoFilters--) | Hämtar en lista med automatiska filter för en Gantt-diagramvy. |
| [getBarRounding()](#getBarRounding--) | Hämtar ett värde som indikerar om staplarna avrundas till närmaste dag. |
| [getBarSize()](#getBarSize--) | Hämtar höjden, i punkter, för Gantt-staplarna i Gantt-diagrammet. |
| [getBarStyles()](#getBarStyles--) | Hämtar en lista med föräldra‑ (gemensamma) stapelstilar för Gantt-diagramvyn. |
| [getBottomTimescaleTier()](#getBottomTimescaleTier--) | Hämtar inställningar för vyns nedre tidsskala-nivå. |
| [getCustomBarStyles()](#getCustomBarStyles--) | Hämtar en lista med anpassade uppgiftsspecifika stapelstilar för Gantt-diagramvyn. |
| [getGridlines()](#getGridlines--) | Hämtar en lista med `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) för Gantt-diagramvyn. |
| [getHideRollupBarsWhenSummaryExpanded()](#getHideRollupBarsWhenSummaryExpanded--) | Hämtar ett värde som indikerar om sammanslagna staplar ska döljas när sammanfattningsuppgiften expanderas. |
| [getMiddleTimescaleTier()](#getMiddleTimescaleTier--) | Hämtar inställningar för vyns mellersta tidsskala-nivå. |
| [getNonWorkingTimeColor()](#getNonWorkingTimeColor--) | Hämtar färg för icke‑arbetstid. |
| [getProgressLines()](#getProgressLines--) | Hämtar förloppslinjer för Gantt-diagramvyn. |
| [getRollUpGanttBars()](#getRollUpGanttBars--) | Hämtar ett värde som indikerar om staplar i Gantt-diagrammet ska rullas upp. |
| [getShowBarSplits()](#getShowBarSplits--) | Hämtar ett värde som indikerar om uppgiftsdelningar i Gantt-diagrammet ska visas. |
| [getShowDrawings()](#getShowDrawings--) | Hämtar ett värde som indikerar om ritningar i Gantt-diagrammet ska visas. |
| [getTableTextStyles()](#getTableTextStyles--) | Hämtar en lista med tabelltextstilar för Gantt-diagramvyn. |
| [getTextStyles()](#getTextStyles--) | Hämtar en lista med [TextStyle](../../com.aspose.tasks/textstyle) för Gantt-diagramvyn. |
| [getTimescaleSizePercentage()](#getTimescaleSizePercentage--) | \{@inheritDoc\} |
| [getTopTimescaleTier()](#getTopTimescaleTier--) | Hämtar inställningar för vyns övre tidsskala-nivå. |
| [setBarRounding(boolean value)](#setBarRounding-boolean-) | Ställer in ett värde som indikerar om staplarna avrundas till närmaste dag. |
| [setBarSize(int value)](#setBarSize-int-) | Ställer in höjden, i punkter, för Gantt-staplarna i Gantt-diagrammet. |
| [setBottomTimescaleTier(TimescaleTier value)](#setBottomTimescaleTier-com.aspose.tasks.TimescaleTier-) | Ställer in inställningar för vyns nedre tidsskala-nivå. |
| [setGridlines(List&lt;Gridlines&gt; value)](#setGridlines-java.util.List-com.aspose.tasks.Gridlines--) | Ställer in en lista med `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) för Gantt-diagramvyn. |
| [setHideRollupBarsWhenSummaryExpanded(boolean value)](#setHideRollupBarsWhenSummaryExpanded-boolean-) | Ställer in ett värde som indikerar om sammanslagna staplar ska döljas när sammanfattningsuppgift expanderas. |
| [setMiddleTimescaleTier(TimescaleTier value)](#setMiddleTimescaleTier-com.aspose.tasks.TimescaleTier-) | Ställer in inställningarna för vyns mellersta tidslinjetier. |
| [setNonWorkingTimeColor(Color value)](#setNonWorkingTimeColor-java.awt.Color-) | Ställer in färg för icke-arbetstid. |
| [setProgressLines(ProgressLines value)](#setProgressLines-com.aspose.tasks.ProgressLines-) | Ställer in förloppslinjer för Gantt-diagramvyn. |
| [setRollUpGanttBars(boolean value)](#setRollUpGanttBars-boolean-) | Ställer in ett värde som indikerar om staplar i Gantt-diagrammet ska rullas upp. |
| [setShowBarSplits(boolean value)](#setShowBarSplits-boolean-) | Ställer in ett värde som indikerar om uppgiftsdelningar i Gantt-diagrammet ska visas. |
| [setShowDrawings(boolean value)](#setShowDrawings-boolean-) | Ställer in ett värde som indikerar om ritningar i Gantt-diagrammet ska visas. |
| [setTextStyles(List&lt;TextStyle&gt; value)](#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--) | Ställer in en lista med [TextStyle](../../com.aspose.tasks/textstyle) för Gantt-diagramvyn. |
| [setTimescaleSizePercentage(int value)](#setTimescaleSizePercentage-int-) | \{@inheritDoc\} |
| [setTopTimescaleTier(TimescaleTier value)](#setTopTimescaleTier-com.aspose.tasks.TimescaleTier-) | Ställer in inställningarna för vyns översta tidslinjetier. |
### GanttChartView() {#GanttChartView--}
```
public GanttChartView()
```


Initierar en ny instans av klassen [GanttChartView](../../com.aspose.tasks/ganttchartview).

### getAutoFilters() {#getAutoFilters--}
```
public final FilterCollection getAutoFilters()
```


Hämtar en lista med automatiska filter för en Gantt-diagramvy.

**Returns:**
[FilterCollection](../../com.aspose.tasks/filtercollection) - a list of auto filters of a Gantt Chart view.
### getBarRounding() {#getBarRounding--}
```
public final boolean getBarRounding()
```


Hämtar ett värde som indikerar om staplarna avrundas till närmaste dag. Standardvärdet är True.

**Returns:**
boolean - ett värde som indikerar om staplarna avrundas till närmaste dag.
### getBarSize() {#getBarSize--}
```
public final int getBarSize()
```


Hämtar höjden, i punkter, för Gantt-staplarna i Gantt-diagrammet.

**Returns:**
int - höjden, i punkter, för Gantt-staplarna i Gantt-diagrammet.
### getBarStyles() {#getBarStyles--}
```
public final List<GanttBarStyle> getBarStyles()
```


Hämtar en lista med föräldra (gemensamma) stapelstilar för Gantt-diagramvyn. [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.GanttBarStyle&gt; - en lista med föräldra (gemensamma) stapelstilar för Gantt-diagramvyn.
### getBottomTimescaleTier() {#getBottomTimescaleTier--}
```
public final TimescaleTier getBottomTimescaleTier()
```


Hämtar inställningarna för vyns nedersta tidslinjetier. [TimescaleTier](../../com.aspose.tasks/timescaletier)

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's bottom timescale tier.
### getCustomBarStyles() {#getCustomBarStyles--}
```
public final List<GanttBarStyle> getCustomBarStyles()
```


Hämtar en lista med anpassade uppgiftsspecifika stapelstilar för Gantt-diagramvyn. [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.GanttBarStyle&gt; - en lista med anpassade uppgiftsspecifika stapelstilar för Gantt-diagramvyn.
### getGridlines() {#getGridlines--}
```
public final List<Gridlines> getGridlines()
```


Hämtar en lista med `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) för Gantt-diagramvyn.

**Returns:**
java.util.List&lt;com.aspose.tasks.Gridlines&gt; - en lista med `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) för Gantt-diagramvyn.
### getHideRollupBarsWhenSummaryExpanded() {#getHideRollupBarsWhenSummaryExpanded--}
```
public final boolean getHideRollupBarsWhenSummaryExpanded()
```


Hämtar ett värde som indikerar om sammanslagna staplar ska döljas när sammanfattningsuppgiften expanderas.

**Returns:**
boolean - ett värde som indikerar om sammanslagna staplar ska döljas när sammanfattningsuppgift expanderas.
### getMiddleTimescaleTier() {#getMiddleTimescaleTier--}
```
public final TimescaleTier getMiddleTimescaleTier()
```


Hämtar inställningarna för vyns mellersta tidslinjetier. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's middle timescale tier.
### getNonWorkingTimeColor() {#getNonWorkingTimeColor--}
```
public final Color getNonWorkingTimeColor()
```


Hämtar färg för icke‑arbetstid.

**Returns:**
java.awt.Color - färg för icke-arbetstid.
### getProgressLines() {#getProgressLines--}
```
public final ProgressLines getProgressLines()
```


Hämtar förloppslinjer för Gantt-diagramvyn. `ProgressLines`([getProgressLines()](../../com.aspose.tasks/ganttchartview\#getProgressLines--)/[setProgressLines(ProgressLines)](../../com.aspose.tasks/ganttchartview\#setProgressLines-ProgressLines-)).

**Returns:**
[ProgressLines](../../com.aspose.tasks/progresslines) - progress lines for the Gantt Chart view.
### getRollUpGanttBars() {#getRollUpGanttBars--}
```
public final boolean getRollUpGanttBars()
```


Hämtar ett värde som indikerar om staplar i Gantt-diagrammet ska rullas upp.

**Returns:**
boolean - ett värde som indikerar om staplar i Gantt-diagrammet ska rullas upp.
### getShowBarSplits() {#getShowBarSplits--}
```
public final boolean getShowBarSplits()
```


Hämtar ett värde som indikerar om uppgiftsdelningar i Gantt-diagrammet ska visas.

**Returns:**
boolean - ett värde som indikerar om uppgiftssplittringar i Gantt-diagrammet ska visas.
### getShowDrawings() {#getShowDrawings--}
```
public final boolean getShowDrawings()
```


Hämtar ett värde som indikerar om ritningar i Gantt-diagrammet ska visas.

**Returns:**
boolean - ett värde som indikerar om ritningar i Gantt-diagrammet ska visas.
### getTableTextStyles() {#getTableTextStyles--}
```
public final List<TableTextStyle> getTableTextStyles()
```


Hämtar en lista med tabelltextstilar för Gantt-diagramvyn. [TableTextStyle](../../com.aspose.tasks/tabletextstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.TableTextStyle&gt; - en lista med tabelltextstilar för Gantt-diagramvyn.
### getTextStyles() {#getTextStyles--}
```
public final List<TextStyle> getTextStyles()
```


Hämtar en lista med [TextStyle](../../com.aspose.tasks/textstyle) för Gantt-diagramvyn.

**Returns:**
java.util.List&lt;com.aspose.tasks.TextStyle&gt; - en lista med [TextStyle](../../com.aspose.tasks/textstyle) för Gantt-diagramvyn.
### getTimescaleSizePercentage() {#getTimescaleSizePercentage--}
```
public final int getTimescaleSizePercentage()
```


Hämtar en procentsats för att minska eller öka avståndet mellan enheter på tidslinjetier.

**Returns:**
int – \{@inheritDoc\}
### getTopTimescaleTier() {#getTopTimescaleTier--}
```
public final TimescaleTier getTopTimescaleTier()
```


Hämtar inställningarna för vyns översta tidslinjetier. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's top timescale tier.
### setBarRounding(boolean value) {#setBarRounding-boolean-}
```
public final void setBarRounding(boolean value)
```


Ställer in ett värde som indikerar om staplarna avrundas till närmaste dag. Standardvärdet är True.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om staplarna avrundas till närmaste dag. |

### setBarSize(int value) {#setBarSize-int-}
```
public final void setBarSize(int value)
```


Ställer in höjden, i punkter, för Gantt-staplarna i Gantt-diagrammet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | höjden, i punkter, för Gantt-staplarna i Gantt-diagrammet. |

### setBottomTimescaleTier(TimescaleTier value) {#setBottomTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setBottomTimescaleTier(TimescaleTier value)
```


Ställer in inställningarna för vyns nedersta tidslinjetier. [TimescaleTier](../../com.aspose.tasks/timescaletier)

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | inställningar för vyns nedersta tidslinjetier. |

### setGridlines(List&lt;Gridlines&gt; value) {#setGridlines-java.util.List-com.aspose.tasks.Gridlines--}
```
public final void setGridlines(List<Gridlines> value)
```


Ställer in en lista med `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) för Gantt-diagramvyn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.Gridlines&gt; | en lista med `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) för Gantt-diagramvyn. |

### setHideRollupBarsWhenSummaryExpanded(boolean value) {#setHideRollupBarsWhenSummaryExpanded-boolean-}
```
public final void setHideRollupBarsWhenSummaryExpanded(boolean value)
```


Ställer in ett värde som indikerar om sammanslagna staplar ska döljas när sammanfattningsuppgift expanderas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om sammanslagna staplar ska döljas när sammanfattningsuppgift expanderas. |

### setMiddleTimescaleTier(TimescaleTier value) {#setMiddleTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setMiddleTimescaleTier(TimescaleTier value)
```


Ställer in inställningarna för vyns mellersta tidslinjetier. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | inställningar för vyns mellersta tidslinjetier. |

### setNonWorkingTimeColor(Color value) {#setNonWorkingTimeColor-java.awt.Color-}
```
public final void setNonWorkingTimeColor(Color value)
```


Ställer in färg för icke-arbetstid.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.awt.Color | färg för icke-arbetstid. |

### setProgressLines(ProgressLines value) {#setProgressLines-com.aspose.tasks.ProgressLines-}
```
public final void setProgressLines(ProgressLines value)
```


Ställer in förloppslinjer för Gantt-diagramvyn. `ProgressLines`([getProgressLines()](../../com.aspose.tasks/ganttchartview\#getProgressLines--)/[setProgressLines(ProgressLines)](../../com.aspose.tasks/ganttchartview\#setProgressLines-ProgressLines-)).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [ProgressLines](../../com.aspose.tasks/progresslines) | förloppslinjer för Gantt-diagramvyn. |

### setRollUpGanttBars(boolean value) {#setRollUpGanttBars-boolean-}
```
public final void setRollUpGanttBars(boolean value)
```


Ställer in ett värde som indikerar om staplar i Gantt-diagrammet ska rullas upp.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om staplar i Gantt-diagrammet ska rullas upp. |

### setShowBarSplits(boolean value) {#setShowBarSplits-boolean-}
```
public final void setShowBarSplits(boolean value)
```


Ställer in ett värde som indikerar om uppgiftsdelningar i Gantt-diagrammet ska visas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om uppgiftssplittringar i Gantt-diagrammet ska visas. |

### setShowDrawings(boolean value) {#setShowDrawings-boolean-}
```
public final void setShowDrawings(boolean value)
```


Ställer in ett värde som indikerar om ritningar i Gantt-diagrammet ska visas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om ritningar i Gantt-diagrammet ska visas. |

### setTextStyles(List&lt;TextStyle&gt; value) {#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--}
```
public final void setTextStyles(List<TextStyle> value)
```


Ställer in en lista med [TextStyle](../../com.aspose.tasks/textstyle) för Gantt-diagramvyn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.TextStyle&gt; | en lista med [TextStyle](../../com.aspose.tasks/textstyle) för Gantt-diagramvyn. |

### setTimescaleSizePercentage(int value) {#setTimescaleSizePercentage-int-}
```
public final void setTimescaleSizePercentage(int value)
```


Ställer in en procentsats för att minska eller öka avståndet mellan enheter på tidslinjetier.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | \{@inheritDoc\} |

### setTopTimescaleTier(TimescaleTier value) {#setTopTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setTopTimescaleTier(TimescaleTier value)
```


Ställer in inställningarna för vyns översta tidslinjetier. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | inställningar för vyns översta tidslinjetier. |

