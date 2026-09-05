---
title: "SaveOptions"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "これは、特定の形式でプロジェクトを保存する際にユーザーが追加オプションを指定できるクラスの抽象基底クラスです。"
type: docs
weight: 274
url: /ja/java/com.aspose.tasks/saveoptions/
---

**Inheritance:**
java.lang.Object、[com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public abstract class SaveOptions extends SimpleSaveOptions
```

これは、特定の形式でプロジェクトを保存する際にユーザーが追加オプションを指定できるクラスの抽象基底クラスです。

--------------------

SaveOptions クラスから派生した任意のクラスのインスタンスは、ストリーム Save または文字列 Save のオーバーロードに渡され、ドキュメントを保存する際にユーザーがカスタムオプションを定義できるようにします。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getBarStyles()](#getBarStyles--) | プロジェクトビューに表示される [BarStyle](../../com.aspose.tasks/barstyle) クラスのインスタンスのリストを取得します。 |
| [getCustomPageSize()](#getCustomPageSize--) | ポイント単位のカスタムページサイズを取得します（1 ポイント = 1/72 インチ）。 |
| [getDrawNonWorkingTime()](#getDrawNonWorkingTime--) | 非稼働時間を描画するかどうかを示す値を取得します（デフォルト値は TRUE）。 |
| [getEndDate()](#getEndDate--) | レンダリングを終了する日付を取得します。 |
| [getFitContent()](#getFitContent--) | 行の高さをコンテンツに合わせて増やすかどうかを示す値を取得します。 |
| [getGridlines()](#getGridlines--) | プロジェクトビューに表示される [Gridline](../../com.aspose.tasks/gridline) のリストを取得します。 |
| [getLegendDrawingOptions()](#getLegendDrawingOptions--) | 凡例の描画方法を定義する値を取得します。 |
| [getLegendItems()](#getLegendItems--) | ページ凡例に描画すべきバーを定義する PageLegendItem の配列を取得します。 |
| [getMarkCriticalTasks()](#getMarkCriticalTasks--) | 重要タスクを赤色で表示するかどうかを示す値を取得します（デフォルト値は FALSE）。 |
| [getNonWorkingTimeColor()](#getNonWorkingTimeColor--) | 非稼働時間の色を取得します。 |
| [getPageCount()](#getPageCount--) | プロジェクトのページ数を取得します。 |
| [getPageSize()](#getPageSize--) | レンダリングされるページのサイズを取得します（デフォルト値は PageSize.A4）。 |
| [getPresentationFormat()](#getPresentationFormat--) | ドキュメントが保存される `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) を取得します。 |
| [getRenderToSinglePage()](#getRenderToSinglePage--) | プロジェクトがグラフィカル形式で保存される際に、単一ページにレンダリングすべきかどうかを示す値を取得します。 |
| [getRollUpGanttBars()](#getRollUpGanttBars--) | サマリタスクバー上のサブタスクをマークすべきかどうかを示す値を取得します。 |
| [getStartDate()](#getStartDate--) | レンダリング開始日を取得します。 |
| [getTaskLinkDrawingCallback()](#getTaskLinkDrawingCallback--) | タスクリンクのレンダリングのいくつかの側面をカスタマイズできるコールバックを取得します。 |
| [getTextStyles()](#getTextStyles--) | プロジェクトビューのレンダリング中に適用されるテキストスタイルの一覧を取得します。 |
| [getTimescale()](#getTimescale--) | `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) の値を取得します。この値は、プロジェクトがグラフィカル形式で保存される際に、タイムスケール（存在する場合）のレンダリング方法を制御するために使用されます。 |
| [getTimescaleFitBehavior()](#getTimescaleFitBehavior--) | タイムスケールの右端をページの端に合わせる方法を定義する動作を取得します。 |
| [getUseGradientBrush()](#getUseGradientBrush--) | ガントチャートのレンダリング時にグラデーションブラシを使用すべきかどうかを示す値を取得します。 |
| [getView()](#getView--) | レンダリングするビュー列の一覧を取得します（[GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)）。 |
| [getViewSettings()](#getViewSettings--) | レンダリングするビュー (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) を取得します。 |
| [isPortrait()](#isPortrait--) | ページの向きが縦向きかどうかを示す値を取得します。ページの向きが横向きの場合は false を返します。 |
| [setBarStyles(List&lt;BarStyle&gt; value)](#setBarStyles-java.util.List-com.aspose.tasks.BarStyle--) | プロジェクトビューに表示される [BarStyle](../../com.aspose.tasks/barstyle) クラスのインスタンスの一覧を設定します。 |
| [setCustomPageSize(Dimension2D value)](#setCustomPageSize-java.awt.geom.Dimension2D-) | カスタムページサイズをポイント単位で設定します（1ポイント = 1/72インチ）。 |
| [setDrawNonWorkingTime(boolean value)](#setDrawNonWorkingTime-boolean-) | 非稼働時間を描画すべきかどうかを示す値を設定します（デフォルトは TRUE）。 |
| [setEndDate(Date value)](#setEndDate-java.util.Date-) | レンダリング終了日を設定します。 |
| [setFitContent(boolean value)](#setFitContent-boolean-) | 行の高さをコンテンツに合わせて拡大すべきかどうかを示す値を設定します。 |
| [setGridlines(List&lt;Gridline&gt; value)](#setGridlines-java.util.List-com.aspose.tasks.Gridline--) | プロジェクトビューに表示される [Gridline](../../com.aspose.tasks/gridline) の一覧を設定します。 |
| [setLegendDrawingOptions(int value)](#setLegendDrawingOptions-int-) | 凡例のレンダリング方法を定義する値を設定します。 |
| [setLegendItems(PageLegendItem[] value)](#setLegendItems-com.aspose.tasks.PageLegendItem---) | ページ凡例にレンダリングすべきバーを定義する PageLegendItem の配列を設定します。 |
| [setMarkCriticalTasks(boolean value)](#setMarkCriticalTasks-boolean-) | 重要タスクを赤色で表示すべきかどうかを示す値を設定します（デフォルトは FALSE）。 |
| [setNonWorkingTimeColor(Color value)](#setNonWorkingTimeColor-java.awt.Color-) | 非稼働時間の色を設定します。 |
| [setPageSize(int value)](#setPageSize-int-) | レンダリングするページサイズを設定します（デフォルトは PageSize.A4）。 |
| [setPortrait(boolean value)](#setPortrait-boolean-) | ページの向きが縦向きかどうかを示す値を設定します。ページの向きが横向きの場合は false を返します。 |
| [setPresentationFormat(int value)](#setPresentationFormat-int-) | ドキュメントが保存される `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) を設定します。 |
| [setRenderToSinglePage(boolean value)](#setRenderToSinglePage-boolean-) | プロジェクトがグラフィカル形式で保存される際に、単一ページにレンダリングすべきかどうかを示す値を設定します。 |
| [setRollUpGanttBars(boolean value)](#setRollUpGanttBars-boolean-) | サマリタスクバー上のサブタスクをマークすべきかどうかを示す値を設定します。 |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | レンダリング開始日を設定します。 |
| [setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value)](#setTaskLinkDrawingCallback-com.aspose.tasks.TaskLinkDrawingCallbackDelegate-) | タスクリンクのレンダリングのいくつかの側面をカスタマイズできるコールバックを設定します。 |
| [setTextStyles(List&lt;TextStyle&gt; value)](#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--) | プロジェクトビューのレンダリング中に適用されるテキストスタイルのリストを設定します。 |
| [setTimescale(int value)](#setTimescale-int-) | プロジェクトがグラフィカル形式で保存されるときに、タイムスケール（存在する場合）のレンダリング方法を制御するために使用される `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) の値を設定します。 |
| [setTimescaleFitBehavior(int value)](#setTimescaleFitBehavior-int-) | タイムスケールの右端をページの端に合わせる方法を定義する動作を設定します。 |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | ガントチャートのレンダリング時にグラデーションブラシを使用するかどうかを示す値を設定します。 |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | レンダリングするビュー列のリストを設定します（[GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)）。 |
| [setViewSettings(View value)](#setViewSettings-com.aspose.tasks.View-) | レンダリングするビュー（`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))）を設定します。 |
### getBarStyles() {#getBarStyles--}
```
public final List<BarStyle> getBarStyles()
```


プロジェクトビューに表示される [BarStyle](../../com.aspose.tasks/barstyle) クラスのインスタンスのリストを取得します。

**Returns:**
java.util.List&lt;com.aspose.tasks.BarStyle&gt; - プロジェクトビューに表示される [BarStyle](../../com.aspose.tasks/barstyle) クラスのインスタンスのリストです。
### getCustomPageSize() {#getCustomPageSize--}
```
public final Dimension2D getCustomPageSize()
```


ポイント単位のカスタムページサイズを取得します（1 ポイント = 1/72 インチ）。

**Returns:**
java.awt.geom.Dimension2D - ポイント単位のカスタムページサイズです（1ポイント = 1/72インチ）。
### getDrawNonWorkingTime() {#getDrawNonWorkingTime--}
```
public final boolean getDrawNonWorkingTime()
```


非稼働時間を描画するかどうかを示す値を取得します（デフォルト値は TRUE）。

**Returns:**
boolean - 非稼働時間を描画するかどうかを示す値です（デフォルト値は TRUE）。
### getEndDate() {#getEndDate--}
```
public final Date getEndDate()
```


レンダリングを終了する日付を取得します。

**Returns:**
java.util.Date - レンダリングを終了する日付です。
### getFitContent() {#getFitContent--}
```
public final boolean getFitContent()
```


行の高さをコンテンツに合わせて増やすかどうかを示す値を取得します。

**Returns:**
boolean - 行の高さをコンテンツに合わせて増やすかどうかを示す値です。
### getGridlines() {#getGridlines--}
```
public final List<Gridline> getGridlines()
```


プロジェクトビューに表示される [Gridline](../../com.aspose.tasks/gridline) のリストを取得します。

**Returns:**
java.util.List&lt;com.aspose.tasks.Gridline&gt; - プロジェクトビューに表示される [Gridline](../../com.aspose.tasks/gridline) のリストです。
### getLegendDrawingOptions() {#getLegendDrawingOptions--}
```
public final int getLegendDrawingOptions()
```


凡例のレンダリング方法を定義する値を取得します。デフォルト値は LegendDrawingOptions.OnEveryPage です。

ガントチャートビューがレンダリングされる場合にのみ適用されます。

**Returns:**
int - 凡例のレンダリング方法を定義する値です。
### getLegendItems() {#getLegendItems--}
```
public final PageLegendItem[] getLegendItems()
```


ページ凡例にレンダリングすべきバーを定義する PageLegendItem の配列を取得します。null の場合、デフォルト項目がレンダリングされます。

ガントチャートビューがレンダリングされる場合にのみ適用されます。

**Returns:**
com.aspose.tasks.PageLegendItem[] - ページ凡例にレンダリングすべきバーを定義する PageLegendItem の配列です。
### getMarkCriticalTasks() {#getMarkCriticalTasks--}
```
public final boolean getMarkCriticalTasks()
```


重要タスクを赤色で表示するかどうかを示す値を取得します（デフォルト値は FALSE）。

**Returns:**
boolean - 重要タスクを赤色で表示するかどうかを示す値です（デフォルト値は FALSE）。
### getNonWorkingTimeColor() {#getNonWorkingTimeColor--}
```
public final Color getNonWorkingTimeColor()
```


非稼働時間の色を取得します。

**Returns:**
java.awt.Color - 非稼働時間の色です。
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


プロジェクトのページ数を取得します。

**Returns:**
int - プロジェクトのページ数です。
### getPageSize() {#getPageSize--}
```
public final int getPageSize()
```


レンダリングされるページのサイズを取得します（デフォルト値は PageSize.A4）。

**Returns:**
int - レンダリングされるページのサイズです（デフォルト値は PageSize.A4）。
### getPresentationFormat() {#getPresentationFormat--}
```
public final int getPresentationFormat()
```


ドキュメントが保存される `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) を取得します。

**Returns:**
int - ドキュメントが保存される `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) の整数値です。
### getRenderToSinglePage() {#getRenderToSinglePage--}
```
public final boolean getRenderToSinglePage()
```


プロジェクトがグラフィカル形式で保存される際に、単一ページにレンダリングすべきかどうかを示す値を取得します。ページサイズは、レンダリングされたプロジェクトが1ページに収まるように変更されます。

**Returns:**
boolean - プロジェクトがグラフィカル形式で保存される際に、単一ページにレンダリングされるかどうかを示す値です。
### getRollUpGanttBars() {#getRollUpGanttBars--}
```
public final boolean getRollUpGanttBars()
```


サマリタスクバー上のサブタスクがマークされるかどうかを示す値を取得します。サブタスクの場合、Rollup フィールドはサブタスクのガントバーの情報がサマリタスクバーにロールアップされるかどうかを示します。サマリタスクの場合、Rollup フィールドはサマリタスクバーがロールアップされたバーを表示するかどうかを示します。サブタスクをロールアップさせるには、サマリタスクの Rollup フィールドを Yes に設定している必要があります。

--------------------

ガントチャートビューがレンダリングされる場合にのみ適用されます。

**Returns:**
boolean - サマリタスクバー上のサブタスクがマークされるかどうかを示す値です。
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


レンダリング開始日を取得します。

**Returns:**
java.util.Date - レンダリング開始日です。
### getTaskLinkDrawingCallback() {#getTaskLinkDrawingCallback--}
```
public final TaskLinkDrawingCallbackDelegate getTaskLinkDrawingCallback()
```


タスクリンクのレンダリングのいくつかの側面をカスタマイズできるコールバックを取得します。

ガントチャートビューがレンダリングされる場合にのみ適用されます。

**Returns:**
[TaskLinkDrawingCallbackDelegate](../../com.aspose.tasks/tasklinkdrawingcallbackdelegate) - a callback that can be used to customize some aspects of task links rendering.
### getTextStyles() {#getTextStyles--}
```
public final List<TextStyle> getTextStyles()
```


プロジェクトビューのレンダリング中に適用されるテキストスタイルの一覧を取得します。

--------------------

これらのスタイルは GanttCharView.setTextStyles で定義されたスタイルを上書きします。

**Returns:**
java.util.List&lt;com.aspose.tasks.TextStyle&gt; - プロジェクトビューのレンダリング中に適用されるテキストスタイルのリストです。
### getTimescale() {#getTimescale--}
```
public final int getTimescale()
```


`Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) の値を取得します。この値は、プロジェクトがグラフィカル形式で保存される際に、タイムスケール（存在する場合）のレンダリング方法を制御するために使用されます。

**Returns:**
int - `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) の値で、プロジェクトがグラフィカル形式で保存される際に、タイムスケール（存在する場合）のレンダリング方法を制御するために使用されます。
### getTimescaleFitBehavior() {#getTimescaleFitBehavior--}
```
public final int getTimescaleFitBehavior()
```


タイムスケールの右端をページの端に合わせる方法を定義する動作を取得します。

**Returns:**
int - タイムスケールの右端をページの端に合わせる方法を定義する動作です。
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


ガントチャートのレンダリング時にグラデーションブラシを使用すべきかどうかを示す値を取得します。

--------------------

ガントチャートビューがレンダリングされる場合にのみ適用されます。

**Returns:**
boolean - ガントチャートのレンダリング時にグラデーションブラシを使用するかどうかを示す値です。
### getView() {#getView--}
```
public final ProjectView getView()
```


レンダリングするビュー列のリストを取得します ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn))。設定されていない場合、タスク ID、タスク名、開始日と終了日だけがレンダリングされます。View と `ViewSettings`([getViewSettings()](../../com.aspose.tasks/saveoptions\#getViewSettings--)/[setViewSettings(View)](../../com.aspose.tasks/saveoptions\#setViewSettings-View-)) の両方のプロパティが設定されている場合、View の列が ViewSettings の列を上書きします。

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns to render ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)).
### getViewSettings() {#getViewSettings--}
```
public final View getViewSettings()
```


レンダリングするビュー (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) を取得します。このオプションを使用して、PDF、HTML、または画像形式で保存すべきビューを明示的に指定できます。このプロパティが設定されている場合、プロジェクト保存時に [PresentationFormat](../../com.aspose.tasks/presentationformat) プロパティは無視されます。ビューは以下のいずれかの画面から選択する必要があります ((`Aspose.Tasks.View.Screen`([View.getScreen()](../../com.aspose.tasks/view\#getScreen--)/[View.setScreen(int)](../../com.aspose.tasks/view\#setScreen-int-)))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage)

**Returns:**
[View](../../com.aspose.tasks/view) - a view (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) to render.
### isPortrait() {#isPortrait--}
```
public final boolean isPortrait()
```


ページの向きが縦向きかどうかを示す値を取得します。ページの向きが横向きの場合は false を返します。

--------------------

SaveOptions.getPageSize() == PageSize.DefinedInView の場合は適用されません。この場合は [PageSettings.isPortrait()](../../com.aspose.tasks/pagesettings\#isPortrait--) が代わりに使用されます。[getCustomPageSize()](../../com.aspose.tasks/saveoptions\#getCustomPageSize--) が設定されている場合も適用されません。

**Returns:**
boolean - ページの向きが縦向きかどうかを示す値です。横向きの場合は false を返します。
### setBarStyles(List&lt;BarStyle&gt; value) {#setBarStyles-java.util.List-com.aspose.tasks.BarStyle--}
```
public final void setBarStyles(List<BarStyle> value)
```


プロジェクトビューに表示される [BarStyle](../../com.aspose.tasks/barstyle) クラスのインスタンスの一覧を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.BarStyle&gt; | プロジェクトビューに表示される [BarStyle](../../com.aspose.tasks/barstyle) クラスのインスタンスのリストです。 |

### setCustomPageSize(Dimension2D value) {#setCustomPageSize-java.awt.geom.Dimension2D-}
```
public final void setCustomPageSize(Dimension2D value)
```


カスタムページサイズをポイント単位で設定します（1ポイント = 1/72インチ）。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.awt.geom.Dimension2D | ポイント単位のカスタムページサイズです（1 ポイント = 1/72 インチ）。 |

### setDrawNonWorkingTime(boolean value) {#setDrawNonWorkingTime-boolean-}
```
public final void setDrawNonWorkingTime(boolean value)
```


非稼働時間を描画すべきかどうかを示す値を設定します（デフォルトは TRUE）。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | 非稼働時間を描画するかどうかを示す値です（デフォルト値は TRUE）。 |

### setEndDate(Date value) {#setEndDate-java.util.Date-}
```
public final void setEndDate(Date value)
```


レンダリング終了日を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | レンダリング終了日です。 |

### setFitContent(boolean value) {#setFitContent-boolean-}
```
public final void setFitContent(boolean value)
```


行の高さをコンテンツに合わせて拡大すべきかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | 行の高さを内容に合わせて増やすかどうかを示す値です。 |

### setGridlines(List&lt;Gridline&gt; value) {#setGridlines-java.util.List-com.aspose.tasks.Gridline--}
```
public final void setGridlines(List<Gridline> value)
```


プロジェクトビューに表示される [Gridline](../../com.aspose.tasks/gridline) の一覧を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.Gridline&gt; | プロジェクトビューに表示される [Gridline](../../com.aspose.tasks/gridline) のリストです。 |

### setLegendDrawingOptions(int value) {#setLegendDrawingOptions-int-}
```
public final void setLegendDrawingOptions(int value)
```


凡例の描画方法を定義する値を設定します。デフォルト値は LegendDrawingOptions.OnEveryPage です。

ガントチャートビューがレンダリングされる場合にのみ適用されます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 凡例の描画方法を定義する値です。 |

### setLegendItems(PageLegendItem[] value) {#setLegendItems-com.aspose.tasks.PageLegendItem---}
```
public final void setLegendItems(PageLegendItem[] value)
```


ページ凡例にレンダリングすべきバーを定義する PageLegendItem の配列を設定します。null の場合、デフォルト項目がレンダリングされます。

ガントチャートビューがレンダリングされる場合にのみ適用されます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [PageLegendItem\[\]](../../com.aspose.tasks/pagelegenditem) | ページ凡例にレンダリングすべきバーを定義する PageLegendItem の配列です。 |

### setMarkCriticalTasks(boolean value) {#setMarkCriticalTasks-boolean-}
```
public final void setMarkCriticalTasks(boolean value)
```


重要タスクを赤色で表示すべきかどうかを示す値を設定します（デフォルトは FALSE）。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | 重要タスクを赤色で表示するかどうかを示す値です（デフォルト値は FALSE）。 |

### setNonWorkingTimeColor(Color value) {#setNonWorkingTimeColor-java.awt.Color-}
```
public final void setNonWorkingTimeColor(Color value)
```


非稼働時間の色を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.awt.Color | 非稼働時間の色です。 |

### setPageSize(int value) {#setPageSize-int-}
```
public final void setPageSize(int value)
```


レンダリングするページサイズを設定します（デフォルトは PageSize.A4）。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | レンダリングされるページのサイズ（デフォルト値は PageSize.A4）。 |

### setPortrait(boolean value) {#setPortrait-boolean-}
```
public final void setPortrait(boolean value)
```


ページの向きが縦向きかどうかを示す値を設定します。ページの向きが横向きの場合は false を返します。

--------------------

SaveOptions.PageSize == Visualization.PageSize.DefinedInView の場合は適用されません。この場合は [PageSettings.setPortrait(boolean)](../../com.aspose.tasks/pagesettings\#setPortrait-boolean-) が代わりに使用されます。[getCustomPageSize()](../../com.aspose.tasks/saveoptions\#getCustomPageSize--) が設定されている場合も適用されません。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | ページの向きが縦向きかどうかを示す値です。横向きの場合は false を返します。 |

### setPresentationFormat(int value) {#setPresentationFormat-int-}
```
public final void setPresentationFormat(int value)
```


ドキュメントが保存される `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | int | ドキュメントが保存される `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-))。 |

### setRenderToSinglePage(boolean value) {#setRenderToSinglePage-boolean-}
```
public final void setRenderToSinglePage(boolean value)
```


プロジェクトがグラフィカル形式で保存される際に、単一ページにレンダリングするかどうかを示す値を設定します。ページサイズが変更され、レンダリングされたプロジェクトが1ページに収まるようになります。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | プロジェクトがグラフィカル形式で保存される際に、単一ページにレンダリングするかどうかを示す値です。 |

### setRollUpGanttBars(boolean value) {#setRollUpGanttBars-boolean-}
```
public final void setRollUpGanttBars(boolean value)
```


サマリタスクバー上のサブタスクをマークするかどうかを示す値を設定します。サブタスクの場合、Rollup フィールドはサブタスクのガントバーの情報がサマリタスクバーにロールアップされるかどうかを示します。サマリタスクの場合、Rollup フィールドはサマリタスクバーがロールアップされたバーを表示するかどうかを示します。サブタスクをロールアップさせるには、サマリタスクの Rollup フィールドを Yes に設定している必要があります。

--------------------

ガントチャートビューがレンダリングされる場合にのみ適用されます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | サマリタスクバー上のサブタスクをマークするかどうかを示す値です。 |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


レンダリング開始日を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | レンダリング開始日です。 |

### setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value) {#setTaskLinkDrawingCallback-com.aspose.tasks.TaskLinkDrawingCallbackDelegate-}
```
public final void setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value)
```


タスクリンクのレンダリングのいくつかの側面をカスタマイズできるコールバックを設定します。

ガントチャートビューがレンダリングされる場合にのみ適用されます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [TaskLinkDrawingCallbackDelegate](../../com.aspose.tasks/tasklinkdrawingcallbackdelegate) | タスクリンクのレンダリングのいくつかの側面をカスタマイズできるコールバックです。 |

### setTextStyles(List&lt;TextStyle&gt; value) {#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--}
```
public final void setTextStyles(List<TextStyle> value)
```


プロジェクトビューのレンダリング中に適用されるテキストスタイルのリストを設定します。

--------------------

これらのスタイルは GanttCharView.setTextStyles で定義されたスタイルを上書きします。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.List&lt;com.aspose.tasks.TextStyle&gt; | プロジェクトビューのレンダリング中に適用されるテキストスタイルのリストです。 |

### setTimescale(int value) {#setTimescale-int-}
```
public final void setTimescale(int value)
```


プロジェクトがグラフィカル形式で保存されるときに、タイムスケール（存在する場合）のレンダリング方法を制御するために使用される `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | int | `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) の値で、プロジェクトがグラフィカル形式で保存される際に、タイムスケール（存在する場合）のレンダリング方法を制御するために使用されます。 |

### setTimescaleFitBehavior(int value) {#setTimescaleFitBehavior-int-}
```
public final void setTimescaleFitBehavior(int value)
```


タイムスケールの右端をページの端に合わせる方法を定義する動作を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | タイムスケールの右端をページの端に合わせる方法を定義する動作です。 |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


ガントチャートのレンダリング時にグラデーションブラシを使用するかどうかを示す値を設定します。

--------------------

ガントチャートビューがレンダリングされる場合にのみ適用されます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | ガントチャートのレンダリング時にグラデーションブラシを使用するかどうかを示す値です。 |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


レンダリングするビュー列のリストを設定します（[GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)）。設定しない場合、タスク ID、タスク名、開始日と終了日だけがレンダリングされます。View と `ViewSettings`([getViewSettings()](../../com.aspose.tasks/saveoptions\#getViewSettings--)/[setViewSettings(View)](../../com.aspose.tasks/saveoptions\#setViewSettings-View-)) の両方のプロパティが設定されている場合、View の列が ViewSettings の列を上書きします。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | レンダリングするビュー列のリストです（[GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)）。 |

### setViewSettings(View value) {#setViewSettings-com.aspose.tasks.View-}
```
public final void setViewSettings(View value)
```


レンダリングするビューとして `View`（`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))）を設定します。このオプションを使用して、PDF、HTML、または画像形式で保存するビューを明示的に指定できます。このプロパティが設定されている場合、プロジェクトが保存される際に [PresentationFormat](../../com.aspose.tasks/presentationformat) プロパティは無視されます。ビューは次のいずれかのスクリーンから選択する必要があります（`Aspose.Tasks.View.Screen`([View.getScreen()](../../com.aspose.tasks/view\#getScreen--)/[View.setScreen(int)](../../com.aspose.tasks/view\#setScreen-int-))）：Gantt、TaskSheet、TaskUsage、ResourceSheet、ResourceUsage。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [View](../../com.aspose.tasks/view) | レンダリングするビュー（`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))）です。 |

