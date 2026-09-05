---
title: "GanttChartView"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "ガントチャートビューを表します。"
type: docs
weight: 112
url: /ja/java/com.aspose.tasks/ganttchartview/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.View](../../com.aspose.tasks/view)

**All Implemented Interfaces:**
com.aspose.tasks.ITimescaledView
```
public class GanttChartView extends View implements ITimescaledView
```

ガントチャートビューを表します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [GanttChartView()](#GanttChartView--) | [GanttChartView](../../com.aspose.tasks/ganttchartview) クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getAutoFilters()](#getAutoFilters--) | Gantt Chartビューの自動フィルターの一覧を取得します。 |
| [getBarRounding()](#getBarRounding--) | バーが最も近い日に丸められるかどうかを示す値を取得します。 |
| [getBarSize()](#getBarSize--) | Gantt Chartのガントバーの高さ（ポイント単位）を取得します。 |
| [getBarStyles()](#getBarStyles--) | Gantt Chartビューの親（共通）バー スタイルの一覧を取得します。 |
| [getBottomTimescaleTier()](#getBottomTimescaleTier--) | ビューの下部タイムスケール層の設定を取得します。 |
| [getCustomBarStyles()](#getCustomBarStyles--) | Gantt Chartビューのカスタムタスク固有バー スタイルの一覧を取得します。 |
| [getGridlines()](#getGridlines--) | Gantt Chartビューの`Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--))の一覧を取得します。 |
| [getHideRollupBarsWhenSummaryExpanded()](#getHideRollupBarsWhenSummaryExpanded--) | サマリータスクを展開したときにロールアップバーを非表示にするかどうかを示す値を取得します。 |
| [getMiddleTimescaleTier()](#getMiddleTimescaleTier--) | ビューの中間タイムスケール層の設定を取得します。 |
| [getNonWorkingTimeColor()](#getNonWorkingTimeColor--) | 非稼働時間の色を取得します。 |
| [getProgressLines()](#getProgressLines--) | Gantt Chartビューの進行ラインを取得します。 |
| [getRollUpGanttBars()](#getRollUpGanttBars--) | Gantt Chart上のバーをロールアップする必要があるかどうかを示す値を取得します。 |
| [getShowBarSplits()](#getShowBarSplits--) | Gantt Chart上のタスク分割を表示する必要があるかどうかを示す値を取得します。 |
| [getShowDrawings()](#getShowDrawings--) | Gantt Chart上の図面を表示する必要があるかどうかを示す値を取得します。 |
| [getTableTextStyles()](#getTableTextStyles--) | Gantt Chartビューのテーブルテキストスタイルの一覧を取得します。 |
| [getTextStyles()](#getTextStyles--) | Gantt Chartビューの[TextStyle](../../com.aspose.tasks/textstyle)の一覧を取得します。 |
| [getTimescaleSizePercentage()](#getTimescaleSizePercentage--) | \{@inheritDoc\} |
| [getTopTimescaleTier()](#getTopTimescaleTier--) | ビューの上部タイムスケール層の設定を取得します。 |
| [setBarRounding(boolean value)](#setBarRounding-boolean-) | バーが最も近い日に丸められるかどうかを示す値を設定します。 |
| [setBarSize(int value)](#setBarSize-int-) | Gantt Chartのガントバーの高さ（ポイント単位）を設定します。 |
| [setBottomTimescaleTier(TimescaleTier value)](#setBottomTimescaleTier-com.aspose.tasks.TimescaleTier-) | ビューの下部タイムスケール層の設定を設定します。 |
| [setGridlines(List&lt;Gridlines&gt; value)](#setGridlines-java.util.List-com.aspose.tasks.Gridlines--) | Gantt Chartビューの`Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--))の一覧を設定します。 |
| [setHideRollupBarsWhenSummaryExpanded(boolean value)](#setHideRollupBarsWhenSummaryExpanded-boolean-) | サマリータスクを展開したときにロールアップバーを非表示にするかどうかを示す値を設定します。 |
| [setMiddleTimescaleTier(TimescaleTier value)](#setMiddleTimescaleTier-com.aspose.tasks.TimescaleTier-) | ビューの中間タイムスケール層の設定を設定します。 |
| [setNonWorkingTimeColor(Color value)](#setNonWorkingTimeColor-java.awt.Color-) | 非稼働時間の色を設定します。 |
| [setProgressLines(ProgressLines value)](#setProgressLines-com.aspose.tasks.ProgressLines-) | Gantt Chartビューの進行ラインを設定します。 |
| [setRollUpGanttBars(boolean value)](#setRollUpGanttBars-boolean-) | Gantt Chart上のバーをロールアップする必要があるかどうかを示す値を設定します。 |
| [setShowBarSplits(boolean value)](#setShowBarSplits-boolean-) | Gantt Chart上のタスク分割を表示する必要があるかどうかを示す値を設定します。 |
| [setShowDrawings(boolean value)](#setShowDrawings-boolean-) | Gantt Chart上の図面を表示する必要があるかどうかを示す値を設定します。 |
| [setTextStyles(List&lt;TextStyle&gt; value)](#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--) | Gantt Chartビューの[TextStyle](../../com.aspose.tasks/textstyle)の一覧を設定します。 |
| [setTimescaleSizePercentage(int value)](#setTimescaleSizePercentage-int-) | \{@inheritDoc\} |
| [setTopTimescaleTier(TimescaleTier value)](#setTopTimescaleTier-com.aspose.tasks.TimescaleTier-) | ビューの上部タイムスケール層の設定を設定します。 |
### GanttChartView() {#GanttChartView--}
```
public GanttChartView()
```


[GanttChartView](../../com.aspose.tasks/ganttchartview) クラスの新しいインスタンスを初期化します。

### getAutoFilters() {#getAutoFilters--}
```
public final FilterCollection getAutoFilters()
```


Gantt Chartビューの自動フィルターの一覧を取得します。

**Returns:**
[FilterCollection](../../com.aspose.tasks/filtercollection) - a list of auto filters of a Gantt Chart view.
### getBarRounding() {#getBarRounding--}
```
public final boolean getBarRounding()
```


バーが最も近い日に丸められるかどうかを示す値を取得します。デフォルト値はTrueです。

**Returns:**
boolean - バーが最も近い日に丸められるかどうかを示す値。
### getBarSize() {#getBarSize--}
```
public final int getBarSize()
```


Gantt Chartのガントバーの高さ（ポイント単位）を取得します。

**Returns:**
int - ガントチャートのガントバーの高さ（ポイント単位）。
### getBarStyles() {#getBarStyles--}
```
public final List<GanttBarStyle> getBarStyles()
```


ガントチャートビューの親（共通）バー スタイルのリストを取得します。 [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.GanttBarStyle&gt; - ガントチャートビューの親（共通）バー スタイルのリスト。
### getBottomTimescaleTier() {#getBottomTimescaleTier--}
```
public final TimescaleTier getBottomTimescaleTier()
```


ビューの下部タイムスケール層の設定を取得します。 [TimescaleTier](../../com.aspose.tasks/timescaletier)

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's bottom timescale tier.
### getCustomBarStyles() {#getCustomBarStyles--}
```
public final List<GanttBarStyle> getCustomBarStyles()
```


ガントチャートビューのカスタムタスク固有バー スタイルのリストを取得します。 [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.GanttBarStyle&gt; - ガントチャートビューのカスタムタスク固有バー スタイルのリスト。
### getGridlines() {#getGridlines--}
```
public final List<Gridlines> getGridlines()
```


Gantt Chartビューの`Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--))の一覧を取得します。

**Returns:**
java.util.List&lt;com.aspose.tasks.Gridlines&gt; - ガントチャートビューの `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) のリスト。
### getHideRollupBarsWhenSummaryExpanded() {#getHideRollupBarsWhenSummaryExpanded--}
```
public final boolean getHideRollupBarsWhenSummaryExpanded()
```


サマリータスクを展開したときにロールアップバーを非表示にするかどうかを示す値を取得します。

**Returns:**
boolean - サマリタスクを展開したときにロールアップバーが非表示になるかどうかを示す値。
### getMiddleTimescaleTier() {#getMiddleTimescaleTier--}
```
public final TimescaleTier getMiddleTimescaleTier()
```


ビューの中間タイムスケール層の設定を取得します。 [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's middle timescale tier.
### getNonWorkingTimeColor() {#getNonWorkingTimeColor--}
```
public final Color getNonWorkingTimeColor()
```


非稼働時間の色を取得します。

**Returns:**
java.awt.Color - 非稼働時間の色。
### getProgressLines() {#getProgressLines--}
```
public final ProgressLines getProgressLines()
```


ガントチャートビューの進捗ラインを取得します。 `ProgressLines`([getProgressLines()](../../com.aspose.tasks/ganttchartview\#getProgressLines--)/[setProgressLines(ProgressLines)](../../com.aspose.tasks/ganttchartview\#setProgressLines-ProgressLines-)).

**Returns:**
[ProgressLines](../../com.aspose.tasks/progresslines) - progress lines for the Gantt Chart view.
### getRollUpGanttBars() {#getRollUpGanttBars--}
```
public final boolean getRollUpGanttBars()
```


Gantt Chart上のバーをロールアップする必要があるかどうかを示す値を取得します。

**Returns:**
boolean - ガントチャート上のバーをロールアップするかどうかを示す値。
### getShowBarSplits() {#getShowBarSplits--}
```
public final boolean getShowBarSplits()
```


Gantt Chart上のタスク分割を表示する必要があるかどうかを示す値を取得します。

**Returns:**
boolean - ガントチャート上のタスク分割を表示するかどうかを示す値。
### getShowDrawings() {#getShowDrawings--}
```
public final boolean getShowDrawings()
```


Gantt Chart上の図面を表示する必要があるかどうかを示す値を取得します。

**Returns:**
boolean - ガントチャート上の図面を表示するかどうかを示す値。
### getTableTextStyles() {#getTableTextStyles--}
```
public final List<TableTextStyle> getTableTextStyles()
```


ガントチャートビューのテーブルテキストスタイルのリストを取得します。 [TableTextStyle](../../com.aspose.tasks/tabletextstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.TableTextStyle&gt; - ガントチャートビューのテーブルテキストスタイルのリスト。
### getTextStyles() {#getTextStyles--}
```
public final List<TextStyle> getTextStyles()
```


Gantt Chartビューの[TextStyle](../../com.aspose.tasks/textstyle)の一覧を取得します。

**Returns:**
java.util.List&lt;com.aspose.tasks.TextStyle&gt; - ガントチャートビューの [TextStyle](../../com.aspose.tasks/textstyle) のリスト。
### getTimescaleSizePercentage() {#getTimescaleSizePercentage--}
```
public final int getTimescaleSizePercentage()
```


タイムスケール層の単位間の間隔を縮小または拡大する割合を取得します。

**Returns:**
int - \{@inheritDoc\}
### getTopTimescaleTier() {#getTopTimescaleTier--}
```
public final TimescaleTier getTopTimescaleTier()
```


ビューの上部タイムスケール層の設定を取得します。 [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's top timescale tier.
### setBarRounding(boolean value) {#setBarRounding-boolean-}
```
public final void setBarRounding(boolean value)
```


バーが最も近い日に丸められるかどうかを示す値を設定します。デフォルト値は True です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | バーが最も近い日に丸められるかどうかを示す値。 |

### setBarSize(int value) {#setBarSize-int-}
```
public final void setBarSize(int value)
```


Gantt Chartのガントバーの高さ（ポイント単位）を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | ガントチャートのガントバーの高さ（ポイント単位）。 |

### setBottomTimescaleTier(TimescaleTier value) {#setBottomTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setBottomTimescaleTier(TimescaleTier value)
```


ビューの下部タイムスケール層の設定を設定します。 [TimescaleTier](../../com.aspose.tasks/timescaletier)

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | ビューの下部タイムスケール層の設定。 |

### setGridlines(List&lt;Gridlines&gt; value) {#setGridlines-java.util.List-com.aspose.tasks.Gridlines--}
```
public final void setGridlines(List<Gridlines> value)
```


Gantt Chartビューの`Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--))の一覧を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.Gridlines&gt; | ガントチャートビューの `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) のリスト。 |

### setHideRollupBarsWhenSummaryExpanded(boolean value) {#setHideRollupBarsWhenSummaryExpanded-boolean-}
```
public final void setHideRollupBarsWhenSummaryExpanded(boolean value)
```


サマリータスクを展開したときにロールアップバーを非表示にするかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | サマリタスクを展開したときにロールアップバーが非表示になるかどうかを示す値。 |

### setMiddleTimescaleTier(TimescaleTier value) {#setMiddleTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setMiddleTimescaleTier(TimescaleTier value)
```


ビューの中間タイムスケール層の設定を設定します。 [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | ビューの中間タイムスケール層の設定。 |

### setNonWorkingTimeColor(Color value) {#setNonWorkingTimeColor-java.awt.Color-}
```
public final void setNonWorkingTimeColor(Color value)
```


非稼働時間の色を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.awt.Color | 非稼働時間の色。 |

### setProgressLines(ProgressLines value) {#setProgressLines-com.aspose.tasks.ProgressLines-}
```
public final void setProgressLines(ProgressLines value)
```


ガントチャートビューの進捗ラインを設定します。 `ProgressLines`([getProgressLines()](../../com.aspose.tasks/ganttchartview\#getProgressLines--)/[setProgressLines(ProgressLines)](../../com.aspose.tasks/ganttchartview\#setProgressLines-ProgressLines-)).

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [ProgressLines](../../com.aspose.tasks/progresslines) | ガントチャートビューの進捗ライン。 |

### setRollUpGanttBars(boolean value) {#setRollUpGanttBars-boolean-}
```
public final void setRollUpGanttBars(boolean value)
```


Gantt Chart上のバーをロールアップする必要があるかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | ガントチャート上のバーをロールアップするかどうかを示す値。 |

### setShowBarSplits(boolean value) {#setShowBarSplits-boolean-}
```
public final void setShowBarSplits(boolean value)
```


Gantt Chart上のタスク分割を表示する必要があるかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | Gantt Chart 上でタスク分割を表示するかどうかを示す値。 |

### setShowDrawings(boolean value) {#setShowDrawings-boolean-}
```
public final void setShowDrawings(boolean value)
```


Gantt Chart上の図面を表示する必要があるかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | Gantt Chart 上の図面を表示するかどうかを示す値。 |

### setTextStyles(List&lt;TextStyle&gt; value) {#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--}
```
public final void setTextStyles(List<TextStyle> value)
```


Gantt Chartビューの[TextStyle](../../com.aspose.tasks/textstyle)の一覧を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.TextStyle&gt; | Gantt Chart ビューの [TextStyle](../../com.aspose.tasks/textstyle) のリスト。 |

### setTimescaleSizePercentage(int value) {#setTimescaleSizePercentage-int-}
```
public final void setTimescaleSizePercentage(int value)
```


タイムスケール層の単位間の間隔を縮小または拡大する割合を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | \{@inheritDoc\} |

### setTopTimescaleTier(TimescaleTier value) {#setTopTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setTopTimescaleTier(TimescaleTier value)
```


ビューの上部タイムスケール層の設定を設定します。 [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | ビューの上部タイムスケール層の設定。 |

