---
title: "ProgressLines"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "ガントチャートビューの進捗ラインを表します。"
type: docs
weight: 219
url: /ja/java/com.aspose.tasks/progresslines/
---

**Inheritance:**
java.lang.Object
```
public class ProgressLines
```

ガントチャートビューの進捗ラインを表します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [ProgressLines()](#ProgressLines--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getBeginAtDate()](#getBeginAtDate--) | プログレスラインの表示開始日を取得します。 |
| [getBeginAtProjectStart()](#getBeginAtProjectStart--) | プロジェクト開始日からプログレスラインを表示するかどうかを示す値を取得します。 |
| [getDateFormat()](#getDateFormat--) | 日付形式を取得します ([DateLabel](../../com.aspose.tasks/datelabel))。 |
| [getDisplayAtCurrentDate()](#getDisplayAtCurrentDate--) | 現在の日付でプログレスラインを表示するかどうかを示す値を取得します。 |
| [getDisplayAtRecurringIntervals()](#getDisplayAtRecurringIntervals--) | 定期的な間隔でプログレスラインを表示するかどうかを示す値を取得します。 |
| [getDisplaySelected()](#getDisplaySelected--) | 選択された日付でプログレスラインを表示するかどうかを示す値を取得します。 |
| [getFont()](#getFont--) | プログレスラインラベルに使用されるフォントを取得します。 |
| [getLineColor()](#getLineColor--) | 現在のプログレスラインの線色を取得します。 |
| [getLinePattern()](#getLinePattern--) | 現在のプログレスラインの線パターンを取得します。 |
| [getOtherLineColor()](#getOtherLineColor--) | 他のプログレスラインの色を取得します。 |
| [getOtherLinePattern()](#getOtherLinePattern--) | 他の進捗ラインの線パターンを取得します。 |
| [getOtherProgressPointColor()](#getOtherProgressPointColor--) | 他の進捗ポイントの色を取得します。 |
| [getOtherProgressPointShape()](#getOtherProgressPointShape--) | 他の進捗ラインの進捗ポイントの形状を取得します。 |
| [getProgressPointColor()](#getProgressPointColor--) | 進捗ポイントの色を取得します。 |
| [getProgressPointShape()](#getProgressPointShape--) | 進捗ポイントの形状を取得します。 |
| [getRecurringInterval()](#getRecurringInterval--) | 繰り返し間隔を取得します。 |
| [getSelectedDates()](#getSelectedDates--) | 進捗ラインを表示するために選択された日付の一覧を取得します。 |
| [getShowDate()](#getShowDate--) | 各進捗ラインに日付を表示するかどうかを示す値を取得します。 |
| [isBaselinePlan()](#isBaselinePlan--) | ベースライン計画または実績の進捗ラインを表示するかどうかを示す値を取得します。 |
| [isBaselinePlan(boolean value)](#isBaselinePlan-boolean-) | ベースライン計画または実績の進捗ラインを表示するかどうかを示す値を設定します。 |
| [setBeginAtDate(Date value)](#setBeginAtDate-java.util.Date-) | 進捗ラインを表示する開始日を設定します。 |
| [setBeginAtProjectStart(boolean value)](#setBeginAtProjectStart-boolean-) | プロジェクト開始日の開始時点から進捗ラインを表示するかどうかを示す値を設定します。 |
| [setDateFormat(int value)](#setDateFormat-int-) | 日付形式を設定します（[DateLabel](../../com.aspose.tasks/datelabel)）。 |
| [setDisplayAtCurrentDate(boolean value)](#setDisplayAtCurrentDate-boolean-) | 現在の日付で進捗ラインを表示するかどうかを示す値を設定します。 |
| [setDisplayAtRecurringIntervals(boolean value)](#setDisplayAtRecurringIntervals-boolean-) | 繰り返し間隔で進捗ラインを表示するかどうかを示す値を設定します。 |
| [setDisplaySelected(boolean value)](#setDisplaySelected-boolean-) | 選択された日付で進捗ラインを表示するかどうかを示す値を設定します。 |
| [setFont(FontDescriptor value)](#setFont-com.aspose.tasks.FontDescriptor-) | 進捗ラインラベルに使用するフォントを設定します。 |
| [setLineColor(Color value)](#setLineColor-java.awt.Color-) | 現在の進捗ラインの線の色を設定します。 |
| [setLinePattern(int value)](#setLinePattern-int-) | 現在の進捗ラインの線パターンを設定します。 |
| [setOtherLineColor(Color value)](#setOtherLineColor-java.awt.Color-) | 他の進捗ラインの色を設定します。 |
| [setOtherLinePattern(int value)](#setOtherLinePattern-int-) | 他の進捗ラインの線パターンを設定します。 |
| [setOtherProgressPointColor(Color value)](#setOtherProgressPointColor-java.awt.Color-) | 他の進捗ポイントの色を設定します。 |
| [setOtherProgressPointShape(int value)](#setOtherProgressPointShape-int-) | 他の進捗ラインの進捗ポイントの形状を設定します。 |
| [setProgressPointColor(Color value)](#setProgressPointColor-java.awt.Color-) | 進捗ポイントの色を設定します。 |
| [setProgressPointShape(int value)](#setProgressPointShape-int-) | 進捗ポイントの形状を設定します。 |
| [setRecurringInterval(RecurringInterval value)](#setRecurringInterval-com.aspose.tasks.RecurringInterval-) | 繰り返し間隔を設定します。 |
| [setShowDate(boolean value)](#setShowDate-boolean-) | 各進捗ラインの日付を表示するかどうかを示す値を設定します。 |
### ProgressLines() {#ProgressLines--}
```
public ProgressLines()
```


### getBeginAtDate() {#getBeginAtDate--}
```
public final Date getBeginAtDate()
```


プログレスラインの表示開始日を取得します。

**Returns:**
java.util.Date - 進捗ラインを表示する日付。
### getBeginAtProjectStart() {#getBeginAtProjectStart--}
```
public final boolean getBeginAtProjectStart()
```


プロジェクト開始日からプログレスラインを表示するかどうかを示す値を取得します。

**Returns:**
boolean - プロジェクト開始日から進捗ラインを表示するかどうかを示す値。
### getDateFormat() {#getDateFormat--}
```
public final int getDateFormat()
```


日付形式を取得します ([DateLabel](../../com.aspose.tasks/datelabel))。

**Returns:**
int - 日付形式（[DateLabel](../../com.aspose.tasks/datelabel)）。
### getDisplayAtCurrentDate() {#getDisplayAtCurrentDate--}
```
public final boolean getDisplayAtCurrentDate()
```


現在の日付でプログレスラインを表示するかどうかを示す値を取得します。

**Returns:**
boolean - 現在の日付で進捗ラインを表示するかどうかを示す値。
### getDisplayAtRecurringIntervals() {#getDisplayAtRecurringIntervals--}
```
public final boolean getDisplayAtRecurringIntervals()
```


定期的な間隔でプログレスラインを表示するかどうかを示す値を取得します。

**Returns:**
boolean - 繰り返し間隔で進捗ラインを表示するかどうかを示す値。
### getDisplaySelected() {#getDisplaySelected--}
```
public final boolean getDisplaySelected()
```


選択された日付でプログレスラインを表示するかどうかを示す値を取得します。

**Returns:**
boolean - 選択された日付で進捗ラインを表示するかどうかを示す値。
### getFont() {#getFont--}
```
public final FontDescriptor getFont()
```


プログレスラインラベルに使用されるフォントを取得します。

**Returns:**
[FontDescriptor](../../com.aspose.tasks/fontdescriptor) - the font used for progress line label.
### getLineColor() {#getLineColor--}
```
public final Color getLineColor()
```


現在のプログレスラインの線色を取得します。

**Returns:**
java.awt.Color - 現在の進捗ラインの線の色。
### getLinePattern() {#getLinePattern--}
```
public final int getLinePattern()
```


現在の進捗ラインの線パターンを取得します。 `LinePattern`([getLinePattern()](../../com.aspose.tasks/progresslines\#getLinePattern--)/[setLinePattern(int)](../../com.aspose.tasks/progresslines\#setLinePattern-int-)).

**Returns:**
int - 現在の進捗ラインの線パターン。
### getOtherLineColor() {#getOtherLineColor--}
```
public final Color getOtherLineColor()
```


他のプログレスラインの色を取得します。

**Returns:**
java.awt.Color - 他の進捗ラインの色。
### getOtherLinePattern() {#getOtherLinePattern--}
```
public final int getOtherLinePattern()
```


他の進捗ラインの線パターンを取得します。

**Returns:**
int - 他の進捗ラインの線パターン。
### getOtherProgressPointColor() {#getOtherProgressPointColor--}
```
public final Color getOtherProgressPointColor()
```


他の進捗ポイントの色を取得します。

**Returns:**
java.awt.Color - 他の進捗ポイントの色。
### getOtherProgressPointShape() {#getOtherProgressPointShape--}
```
public final int getOtherProgressPointShape()
```


他の進捗ラインの進捗ポイントの形状を取得します。

**Returns:**
int - 他の進捗ラインの進捗ポイント形状。
### getProgressPointColor() {#getProgressPointColor--}
```
public final Color getProgressPointColor()
```


進捗ポイントの色を取得します。

**Returns:**
java.awt.Color - 進捗ポイントの色。
### getProgressPointShape() {#getProgressPointShape--}
```
public final int getProgressPointShape()
```


進捗ポイントの形状を取得します。 [GanttBarEndShape](../../com.aspose.tasks/ganttbarendshape)。

**Returns:**
int - 進捗ポイントの形状。
### getRecurringInterval() {#getRecurringInterval--}
```
public final RecurringInterval getRecurringInterval()
```


繰り返し間隔を取得します。 `RecurringInterval`([getRecurringInterval()](../../com.aspose.tasks/progresslines\#getRecurringInterval--)/[setRecurringInterval(RecurringInterval)](../../com.aspose.tasks/progresslines\#setRecurringInterval-RecurringInterval-)).

**Returns:**
[RecurringInterval](../../com.aspose.tasks/recurringinterval) - the recurring interval.
### getSelectedDates() {#getSelectedDates--}
```
public final List<Date> getSelectedDates()
```


進捗ラインを表示するために選択された日付の一覧を取得します。

**Returns:**
java.util.List&lt;java.util.Date&gt; - 進捗ラインを表示するために選択された日付のリスト。
### getShowDate() {#getShowDate--}
```
public final boolean getShowDate()
```


各進捗ラインに日付を表示するかどうかを示す値を取得します。

**Returns:**
boolean - 各進捗ラインの日付を表示するかどうかを示す値。
### isBaselinePlan() {#isBaselinePlan--}
```
public final boolean isBaselinePlan()
```


ベースライン計画または実績の進捗ラインを表示するかどうかを示す値を取得します。

**Returns:**
boolean - ベースライン計画または実績の進捗ラインを表示するかどうかを示す値。
### isBaselinePlan(boolean value) {#isBaselinePlan-boolean-}
```
public final void isBaselinePlan(boolean value)
```


ベースライン計画または実績の進捗ラインを表示するかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | ベースライン計画または実績の進捗ラインを表示するかどうかを示す値。 |

### setBeginAtDate(Date value) {#setBeginAtDate-java.util.Date-}
```
public final void setBeginAtDate(Date value)
```


進捗ラインを表示する開始日を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | 進捗ラインを表示する開始日。 |

### setBeginAtProjectStart(boolean value) {#setBeginAtProjectStart-boolean-}
```
public final void setBeginAtProjectStart(boolean value)
```


プロジェクト開始日の開始時点から進捗ラインを表示するかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | プロジェクト開始日から進捗ラインを表示するかどうかを示す値。 |

### setDateFormat(int value) {#setDateFormat-int-}
```
public final void setDateFormat(int value)
```


日付形式を設定します（[DateLabel](../../com.aspose.tasks/datelabel)）。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | int | 日付形式（[DateLabel](../../com.aspose.tasks/datelabel)）。 |

### setDisplayAtCurrentDate(boolean value) {#setDisplayAtCurrentDate-boolean-}
```
public final void setDisplayAtCurrentDate(boolean value)
```


現在の日付で進捗ラインを表示するかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | 現在の日付に進捗ラインを表示するかどうかを示す値。 |

### setDisplayAtRecurringIntervals(boolean value) {#setDisplayAtRecurringIntervals-boolean-}
```
public final void setDisplayAtRecurringIntervals(boolean value)
```


繰り返し間隔で進捗ラインを表示するかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | 定期的な間隔で進捗ラインを表示するかどうかを示す値。 |

### setDisplaySelected(boolean value) {#setDisplaySelected-boolean-}
```
public final void setDisplaySelected(boolean value)
```


選択された日付で進捗ラインを表示するかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | 選択された日付に進捗ラインを表示するかどうかを示す値。 |

### setFont(FontDescriptor value) {#setFont-com.aspose.tasks.FontDescriptor-}
```
public final void setFont(FontDescriptor value)
```


進捗ラインラベルに使用するフォントを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | 進捗ラインラベルに使用されるフォント。 |

### setLineColor(Color value) {#setLineColor-java.awt.Color-}
```
public final void setLineColor(Color value)
```


現在の進捗ラインの線の色を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.awt.Color | 現在の進捗ラインの線の色。 |

### setLinePattern(int value) {#setLinePattern-int-}
```
public final void setLinePattern(int value)
```


現在の進捗ラインの線パターンを設定します。 `LinePattern`([getLinePattern()](../../com.aspose.tasks/progresslines\#getLinePattern--)/[setLinePattern(int)](../../com.aspose.tasks/progresslines\#setLinePattern-int-)).

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 現在の進捗ラインの線パターン。 |

### setOtherLineColor(Color value) {#setOtherLineColor-java.awt.Color-}
```
public final void setOtherLineColor(Color value)
```


他の進捗ラインの色を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.awt.Color | 他の進捗ラインの色。 |

### setOtherLinePattern(int value) {#setOtherLinePattern-int-}
```
public final void setOtherLinePattern(int value)
```


他の進捗ラインの線パターンを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 他の進捗ラインの線パターン。 |

### setOtherProgressPointColor(Color value) {#setOtherProgressPointColor-java.awt.Color-}
```
public final void setOtherProgressPointColor(Color value)
```


他の進捗ポイントの色を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.awt.Color | 他の進捗ポイントの色。 |

### setOtherProgressPointShape(int value) {#setOtherProgressPointShape-int-}
```
public final void setOtherProgressPointShape(int value)
```


他の進捗ラインの進捗ポイントの形状を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 他の進捗ラインの進捗ポイントの形状。 |

### setProgressPointColor(Color value) {#setProgressPointColor-java.awt.Color-}
```
public final void setProgressPointColor(Color value)
```


進捗ポイントの色を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.awt.Color | 進捗ポイントの色。 |

### setProgressPointShape(int value) {#setProgressPointShape-int-}
```
public final void setProgressPointShape(int value)
```


進捗ポイントの形状を設定します。 [GanttBarEndShape](../../com.aspose.tasks/ganttbarendshape)。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 進捗ポイントの形状。 |

### setRecurringInterval(RecurringInterval value) {#setRecurringInterval-com.aspose.tasks.RecurringInterval-}
```
public final void setRecurringInterval(RecurringInterval value)
```


定期的な間隔を設定します。 `RecurringInterval`([getRecurringInterval()](../../com.aspose.tasks/progresslines\#getRecurringInterval--)/[setRecurringInterval(RecurringInterval)](../../com.aspose.tasks/progresslines\#setRecurringInterval-RecurringInterval-)).

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [RecurringInterval](../../com.aspose.tasks/recurringinterval) | 定期的な間隔。 |

### setShowDate(boolean value) {#setShowDate-boolean-}
```
public final void setShowDate(boolean value)
```


各進捗ラインの日付を表示するかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | 各進捗ラインの日付を表示するかどうかを示す値。 |

