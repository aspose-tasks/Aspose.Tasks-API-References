---
title: "GanttChartView"
second_title: "Aspose.Tasks for Java API Reference"
description: "간트 차트 뷰를 나타냅니다."
type: docs
weight: 112
url: /ko/java/com.aspose.tasks/ganttchartview/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.View](../../com.aspose.tasks/view)

**All Implemented Interfaces:**
com.aspose.tasks.ITimescaledView
```
public class GanttChartView extends View implements ITimescaledView
```

간트 차트 뷰를 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [GanttChartView()](#GanttChartView--) | 새로운 [GanttChartView](../../com.aspose.tasks/ganttchartview) 클래스 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getAutoFilters()](#getAutoFilters--) | Gantt 차트 보기의 자동 필터 목록을 가져옵니다. |
| [getBarRounding()](#getBarRounding--) | 막대가 가장 가까운 날로 반올림되는지 여부를 나타내는 값을 가져옵니다. |
| [getBarSize()](#getBarSize--) | Gantt 차트에서 Gantt 막대의 높이(포인트)를 가져옵니다. |
| [getBarStyles()](#getBarStyles--) | Gantt 차트 보기의 상위(공통) 막대 스타일 목록을 가져옵니다. |
| [getBottomTimescaleTier()](#getBottomTimescaleTier--) | 뷰의 하단 타임스케일 계층 설정을 가져옵니다. |
| [getCustomBarStyles()](#getCustomBarStyles--) | Gantt 차트 보기의 사용자 지정 작업별 막대 스타일 목록을 가져옵니다. |
| [getGridlines()](#getGridlines--) | Gantt 차트 보기의 `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) 목록을 가져옵니다. |
| [getHideRollupBarsWhenSummaryExpanded()](#getHideRollupBarsWhenSummaryExpanded--) | 요약 작업을 확장할 때 롤업 막대가 숨겨지는지 여부를 나타내는 값을 가져옵니다. |
| [getMiddleTimescaleTier()](#getMiddleTimescaleTier--) | 뷰의 중간 타임스케일 계층 설정을 가져옵니다. |
| [getNonWorkingTimeColor()](#getNonWorkingTimeColor--) | 비작업 시간 색상을 가져옵니다. |
| [getProgressLines()](#getProgressLines--) | Gantt 차트 보기의 진행 라인을 가져옵니다. |
| [getRollUpGanttBars()](#getRollUpGanttBars--) | Gantt 차트의 막대를 롤업해야 하는지 여부를 나타내는 값을 가져옵니다. |
| [getShowBarSplits()](#getShowBarSplits--) | Gantt 차트의 작업 분할을 표시해야 하는지 여부를 나타내는 값을 가져옵니다. |
| [getShowDrawings()](#getShowDrawings--) | Gantt 차트의 도면을 표시해야 하는지 여부를 나타내는 값을 가져옵니다. |
| [getTableTextStyles()](#getTableTextStyles--) | Gantt 차트 보기의 표 텍스트 스타일 목록을 가져옵니다. |
| [getTextStyles()](#getTextStyles--) | Gantt 차트 보기의 [TextStyle](../../com.aspose.tasks/textstyle) 목록을 가져옵니다. |
| [getTimescaleSizePercentage()](#getTimescaleSizePercentage--) | \{@inheritDoc\} |
| [getTopTimescaleTier()](#getTopTimescaleTier--) | 뷰의 상단 타임스케일 계층 설정을 가져옵니다. |
| [setBarRounding(boolean value)](#setBarRounding-boolean-) | 막대가 가장 가까운 날로 반올림되는지 여부를 나타내는 값을 설정합니다. |
| [setBarSize(int value)](#setBarSize-int-) | Gantt 차트에서 Gantt 막대의 높이(포인트)를 설정합니다. |
| [setBottomTimescaleTier(TimescaleTier value)](#setBottomTimescaleTier-com.aspose.tasks.TimescaleTier-) | 뷰의 하단 타임스케일 계층 설정을 설정합니다. |
| [setGridlines(List&lt;Gridlines&gt; value)](#setGridlines-java.util.List-com.aspose.tasks.Gridlines--) | Gantt 차트 보기의 `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) 목록을 설정합니다. |
| [setHideRollupBarsWhenSummaryExpanded(boolean value)](#setHideRollupBarsWhenSummaryExpanded-boolean-) | 요약 작업을 확장할 때 롤업 막대가 숨겨지는지 여부를 나타내는 값을 설정합니다. |
| [setMiddleTimescaleTier(TimescaleTier value)](#setMiddleTimescaleTier-com.aspose.tasks.TimescaleTier-) | 보기의 중간 타임스케일 계층 설정을 지정합니다. |
| [setNonWorkingTimeColor(Color value)](#setNonWorkingTimeColor-java.awt.Color-) | 비작업 시간 색상을 설정합니다. |
| [setProgressLines(ProgressLines value)](#setProgressLines-com.aspose.tasks.ProgressLines-) | Gantt 차트 보기의 진행 라인을 설정합니다. |
| [setRollUpGanttBars(boolean value)](#setRollUpGanttBars-boolean-) | Gantt 차트의 막대를 롤업해야 하는지 여부를 나타내는 값을 설정합니다. |
| [setShowBarSplits(boolean value)](#setShowBarSplits-boolean-) | Gantt 차트의 작업 분할을 표시해야 하는지 여부를 나타내는 값을 설정합니다. |
| [setShowDrawings(boolean value)](#setShowDrawings-boolean-) | Gantt 차트의 도면을 표시해야 하는지 여부를 나타내는 값을 설정합니다. |
| [setTextStyles(List&lt;TextStyle&gt; value)](#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--) | Gantt 차트 보기의 [TextStyle](../../com.aspose.tasks/textstyle) 목록을 설정합니다. |
| [setTimescaleSizePercentage(int value)](#setTimescaleSizePercentage-int-) | \{@inheritDoc\} |
| [setTopTimescaleTier(TimescaleTier value)](#setTopTimescaleTier-com.aspose.tasks.TimescaleTier-) | 보기의 상단 타임스케일 계층 설정을 지정합니다. |
### GanttChartView() {#GanttChartView--}
```
public GanttChartView()
```


새로운 [GanttChartView](../../com.aspose.tasks/ganttchartview) 클래스 인스턴스를 초기화합니다.

### getAutoFilters() {#getAutoFilters--}
```
public final FilterCollection getAutoFilters()
```


Gantt 차트 보기의 자동 필터 목록을 가져옵니다.

**Returns:**
[FilterCollection](../../com.aspose.tasks/filtercollection) - a list of auto filters of a Gantt Chart view.
### getBarRounding() {#getBarRounding--}
```
public final boolean getBarRounding()
```


막대가 가장 가까운 날로 반올림되는지 여부를 나타내는 값을 가져옵니다. 기본값은 True입니다.

**Returns:**
boolean - 막대가 가장 가까운 일로 반올림되는지를 나타내는 값.
### getBarSize() {#getBarSize--}
```
public final int getBarSize()
```


Gantt 차트에서 Gantt 막대의 높이(포인트)를 가져옵니다.

**Returns:**
int - Gantt 차트에서 Gantt 막대의 높이(포인트 단위).
### getBarStyles() {#getBarStyles--}
```
public final List<GanttBarStyle> getBarStyles()
```


Gantt 차트 보기의 상위(공통) 막대 스타일 목록을 가져옵니다. [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.GanttBarStyle&gt; - Gantt 차트 보기의 상위(공통) 막대 스타일 목록.
### getBottomTimescaleTier() {#getBottomTimescaleTier--}
```
public final TimescaleTier getBottomTimescaleTier()
```


보기의 하단 타임스케일 계층 설정을 가져옵니다. [TimescaleTier](../../com.aspose.tasks/timescaletier)

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's bottom timescale tier.
### getCustomBarStyles() {#getCustomBarStyles--}
```
public final List<GanttBarStyle> getCustomBarStyles()
```


Gantt 차트 보기의 사용자 지정 작업별 막대 스타일 목록을 가져옵니다. [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.GanttBarStyle&gt; - Gantt 차트 보기의 사용자 지정 작업별 막대 스타일 목록.
### getGridlines() {#getGridlines--}
```
public final List<Gridlines> getGridlines()
```


Gantt 차트 보기의 `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) 목록을 가져옵니다.

**Returns:**
java.util.List&lt;com.aspose.tasks.Gridlines&gt; - Gantt 차트 보기의 `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) 목록.
### getHideRollupBarsWhenSummaryExpanded() {#getHideRollupBarsWhenSummaryExpanded--}
```
public final boolean getHideRollupBarsWhenSummaryExpanded()
```


요약 작업을 확장할 때 롤업 막대가 숨겨지는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 요약 작업을 확장할 때 롤업 막대가 숨겨지는지를 나타내는 값.
### getMiddleTimescaleTier() {#getMiddleTimescaleTier--}
```
public final TimescaleTier getMiddleTimescaleTier()
```


보기의 중간 타임스케일 계층 설정을 가져옵니다. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's middle timescale tier.
### getNonWorkingTimeColor() {#getNonWorkingTimeColor--}
```
public final Color getNonWorkingTimeColor()
```


비작업 시간 색상을 가져옵니다.

**Returns:**
java.awt.Color - 비작업 시간 색상.
### getProgressLines() {#getProgressLines--}
```
public final ProgressLines getProgressLines()
```


Gantt 차트 보기의 진행 라인을 가져옵니다. `ProgressLines`([getProgressLines()](../../com.aspose.tasks/ganttchartview\#getProgressLines--)/[setProgressLines(ProgressLines)](../../com.aspose.tasks/ganttchartview\#setProgressLines-ProgressLines-)).

**Returns:**
[ProgressLines](../../com.aspose.tasks/progresslines) - progress lines for the Gantt Chart view.
### getRollUpGanttBars() {#getRollUpGanttBars--}
```
public final boolean getRollUpGanttBars()
```


Gantt 차트의 막대를 롤업해야 하는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - Gantt 차트의 막대를 롤업해야 하는지를 나타내는 값.
### getShowBarSplits() {#getShowBarSplits--}
```
public final boolean getShowBarSplits()
```


Gantt 차트의 작업 분할을 표시해야 하는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - Gantt 차트에서 작업 분할을 표시해야 하는지를 나타내는 값.
### getShowDrawings() {#getShowDrawings--}
```
public final boolean getShowDrawings()
```


Gantt 차트의 도면을 표시해야 하는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - Gantt 차트에서 도면을 표시해야 하는지를 나타내는 값.
### getTableTextStyles() {#getTableTextStyles--}
```
public final List<TableTextStyle> getTableTextStyles()
```


Gantt 차트 보기의 표 텍스트 스타일 목록을 가져옵니다. [TableTextStyle](../../com.aspose.tasks/tabletextstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.TableTextStyle&gt; - Gantt 차트 보기의 표 텍스트 스타일 목록.
### getTextStyles() {#getTextStyles--}
```
public final List<TextStyle> getTextStyles()
```


Gantt 차트 보기의 [TextStyle](../../com.aspose.tasks/textstyle) 목록을 가져옵니다.

**Returns:**
java.util.List&lt;com.aspose.tasks.TextStyle&gt; - Gantt 차트 보기의 [TextStyle](../../com.aspose.tasks/textstyle) 목록.
### getTimescaleSizePercentage() {#getTimescaleSizePercentage--}
```
public final int getTimescaleSizePercentage()
```


타임스케일 계층에서 단위 간 간격을 줄이거나 늘릴 비율을 가져옵니다.

**Returns:**
int - \{@inheritDoc\}
### getTopTimescaleTier() {#getTopTimescaleTier--}
```
public final TimescaleTier getTopTimescaleTier()
```


보기의 상단 타임스케일 계층 설정을 가져옵니다. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's top timescale tier.
### setBarRounding(boolean value) {#setBarRounding-boolean-}
```
public final void setBarRounding(boolean value)
```


막대가 가장 가까운 일로 반올림되는지를 나타내는 값을 설정합니다. 기본값은 True입니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 막대가 가장 가까운 일로 반올림되는지를 나타내는 값. |

### setBarSize(int value) {#setBarSize-int-}
```
public final void setBarSize(int value)
```


Gantt 차트에서 Gantt 막대의 높이(포인트)를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | Gantt 차트에서 Gantt 막대의 높이(포인트 단위). |

### setBottomTimescaleTier(TimescaleTier value) {#setBottomTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setBottomTimescaleTier(TimescaleTier value)
```


보기의 하단 타임스케일 계층 설정을 지정합니다. [TimescaleTier](../../com.aspose.tasks/timescaletier)

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | 보기의 하단 타임스케일 계층 설정. |

### setGridlines(List&lt;Gridlines&gt; value) {#setGridlines-java.util.List-com.aspose.tasks.Gridlines--}
```
public final void setGridlines(List<Gridlines> value)
```


Gantt 차트 보기의 `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) 목록을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.Gridlines&gt; | Gantt 차트 보기의 `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) 목록. |

### setHideRollupBarsWhenSummaryExpanded(boolean value) {#setHideRollupBarsWhenSummaryExpanded-boolean-}
```
public final void setHideRollupBarsWhenSummaryExpanded(boolean value)
```


요약 작업을 확장할 때 롤업 막대가 숨겨지는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 요약 작업을 확장할 때 롤업 막대가 숨겨지는지를 나타내는 값. |

### setMiddleTimescaleTier(TimescaleTier value) {#setMiddleTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setMiddleTimescaleTier(TimescaleTier value)
```


보기의 중간 타임스케일 계층 설정을 지정합니다. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | 보기의 중간 타임스케일 계층 설정. |

### setNonWorkingTimeColor(Color value) {#setNonWorkingTimeColor-java.awt.Color-}
```
public final void setNonWorkingTimeColor(Color value)
```


비작업 시간 색상을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.awt.Color | 비작업 시간 색상. |

### setProgressLines(ProgressLines value) {#setProgressLines-com.aspose.tasks.ProgressLines-}
```
public final void setProgressLines(ProgressLines value)
```


Gantt 차트 보기의 진행 라인을 설정합니다. `ProgressLines`([getProgressLines()](../../com.aspose.tasks/ganttchartview\#getProgressLines--)/[setProgressLines(ProgressLines)](../../com.aspose.tasks/ganttchartview\#setProgressLines-ProgressLines-)).

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [ProgressLines](../../com.aspose.tasks/progresslines) | Gantt 차트 보기의 진행 라인. |

### setRollUpGanttBars(boolean value) {#setRollUpGanttBars-boolean-}
```
public final void setRollUpGanttBars(boolean value)
```


Gantt 차트의 막대를 롤업해야 하는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | Gantt 차트의 막대를 롤업해야 하는지를 나타내는 값. |

### setShowBarSplits(boolean value) {#setShowBarSplits-boolean-}
```
public final void setShowBarSplits(boolean value)
```


Gantt 차트의 작업 분할을 표시해야 하는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | Gantt 차트에서 작업 분할을 표시할지 여부를 나타내는 값. |

### setShowDrawings(boolean value) {#setShowDrawings-boolean-}
```
public final void setShowDrawings(boolean value)
```


Gantt 차트의 도면을 표시해야 하는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | Gantt 차트에서 도면을 표시할지 여부를 나타내는 값. |

### setTextStyles(List&lt;TextStyle&gt; value) {#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--}
```
public final void setTextStyles(List<TextStyle> value)
```


Gantt 차트 보기의 [TextStyle](../../com.aspose.tasks/textstyle) 목록을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.TextStyle&gt; | Gantt 차트 보기의 [TextStyle](../../com.aspose.tasks/textstyle) 목록. |

### setTimescaleSizePercentage(int value) {#setTimescaleSizePercentage-int-}
```
public final void setTimescaleSizePercentage(int value)
```


타임스케일 계층에서 단위 간 간격을 줄이거나 늘릴 비율을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | \{@inheritDoc\} |

### setTopTimescaleTier(TimescaleTier value) {#setTopTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setTopTimescaleTier(TimescaleTier value)
```


보기의 상단 타임스케일 계층 설정을 지정합니다. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | 보기의 상단 타임스케일 계층 설정. |

