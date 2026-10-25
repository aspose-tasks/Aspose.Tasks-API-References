---
title: "VisualObjectPlacement"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "ビュー内の  の配置と外観を表します。"
type: docs
weight: 346
url: /ja/java/com.aspose.tasks/visualobjectplacement/
---

**Inheritance:**
java.lang.Object
```
public final class VisualObjectPlacement
```

ビュー内の [OleObject](../../com.aspose/tasks/oleobject) の配置と外観を表します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [VisualObjectPlacement()](#VisualObjectPlacement--) | 新しい [VisualObjectPlacement](../../com.aspose/tasks/visualobjectplacement) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getAttachmentPoint()](#getAttachmentPoint--) | 「タスクに添付」オプションが選択されたときの、タスクに対するビジュアルオブジェクトの配置を取得します。 |
| [getBorderLineColor()](#getBorderLineColor--) | 境界線の色を取得します。 |
| [getBorderLineThickness()](#getBorderLineThickness--) | 境界線の太さを取得します（許容値は0〜5です）。 |
| [getFillColor()](#getFillColor--) | 塗りつぶしの色を取得します。 |
| [getFillPattern()](#getFillPattern--) | 塗りつぶしパターンを取得します。 |
| [getHeight()](#getHeight--) | 表示されるビジュアルオブジェクトの高さを取得します。 |
| [getHorizontalOffset()](#getHorizontalOffset--) | ビジュアルオブジェクトの水平オフセットを取得します。 |
| [getOleObjectId()](#getOleObjectId--) | [OleObject](../../com.aspose.tasks/oleobject) オブジェクトの Id を取得します。 |
| [getTaskId()](#getTaskId--) | タスクに 'Attach to task' オプションが選択されている場合はタスクの Id を取得し、そうでない場合は -1 を返します。 |
| [getTimescaleDate()](#getTimescaleDate--) | 'Attach to timescale' オプションが選択されている場合のビジュアルオブジェクトの日付配置を取得します。 |
| [getVerticalOffset()](#getVerticalOffset--) | ビジュアルオブジェクトの垂直オフセットを取得します。 |
| [getWidth()](#getWidth--) | 表示されるビジュアルオブジェクトの幅を取得します。 |
| [setAttachmentPoint(int value)](#setAttachmentPoint-int-) | 'Attach to task' オプションが選択されている場合、タスクに対するビジュアルオブジェクトの配置を設定します。 |
| [setBorderLineColor(Color value)](#setBorderLineColor-java.awt.Color-) | 境界線の色を設定します。 |
| [setBorderLineThickness(byte value)](#setBorderLineThickness-byte-) | 境界線の太さを設定します（許容値は0〜5です）。 |
| [setFillColor(Color value)](#setFillColor-java.awt.Color-) | 塗りつぶしの色を設定します。 |
| [setFillPattern(int value)](#setFillPattern-int-) | 塗りつぶしパターンを設定します。 |
| [setHeight(double value)](#setHeight-double-) | 表示されるビジュアルオブジェクトの高さを設定します。 |
| [setHorizontalOffset(double value)](#setHorizontalOffset-double-) | ビジュアルオブジェクトの水平オフセットを設定します。 |
| [setOleObjectId(int value)](#setOleObjectId-int-) | [OleObject](../../com.aspose.tasks/oleobject) オブジェクトの Id を設定します。 |
| [setTaskId(int value)](#setTaskId-int-) | 'Attach to task' オプションが選択されている場合はタスクの Id を設定し、そうでない場合は -1 を設定します。 |
| [setTimescaleDate(Date value)](#setTimescaleDate-java.util.Date-) | 'Attach to timescale' オプションが選択されている場合、ビジュアルオブジェクトの日付配置を設定します。 |
| [setVerticalOffset(double value)](#setVerticalOffset-double-) | ビジュアルオブジェクトの垂直オフセットを設定します。 |
| [setWidth(double value)](#setWidth-double-) | 表示されるビジュアルオブジェクトの幅を設定します。 |
### VisualObjectPlacement() {#VisualObjectPlacement--}
```
public VisualObjectPlacement()
```


新しい [VisualObjectPlacement](../../com.aspose/tasks/visualobjectplacement) クラスのインスタンスを初期化します。

### getAttachmentPoint() {#getAttachmentPoint--}
```
public final int getAttachmentPoint()
```


「タスクに添付」オプションが選択されたときの、タスクに対するビジュアルオブジェクトの配置を取得します。

**Returns:**
int - 'Attach to task' オプションが選択されている場合のタスクに対するビジュアルオブジェクトの配置。
### getBorderLineColor() {#getBorderLineColor--}
```
public final Color getBorderLineColor()
```


境界線の色を取得します。

**Returns:**
java.awt.Color - 境界線の色。
### getBorderLineThickness() {#getBorderLineThickness--}
```
public final byte getBorderLineThickness()
```


境界線の太さを取得します（許容値は0〜5です）。

**Returns:**
byte - 境界線の太さ（許容値は 0〜5）。
### getFillColor() {#getFillColor--}
```
public final Color getFillColor()
```


塗りつぶしの色を取得します。

**Returns:**
java.awt.Color - 塗りつぶし色。
### getFillPattern() {#getFillPattern--}
```
public final int getFillPattern()
```


塗りつぶしパターンを取得します。

**Returns:**
int - 塗りつぶしパターン。
### getHeight() {#getHeight--}
```
public final double getHeight()
```


表示されるビジュアルオブジェクトの高さを取得します。

**Returns:**
double - ビジュアルオブジェクトの表示高さ。
### getHorizontalOffset() {#getHorizontalOffset--}
```
public final double getHorizontalOffset()
```


ビジュアルオブジェクトの水平オフセットを取得します。

**Returns:**
double - ビジュアルオブジェクトの水平オフセット。
### getOleObjectId() {#getOleObjectId--}
```
public final int getOleObjectId()
```


[OleObject](../../com.aspose.tasks/oleobject) オブジェクトの Id を取得します。

**Returns:**
int - [OleObject](../../com.aspose/tasks/oleobject) オブジェクトの ID。
### getTaskId() {#getTaskId--}
```
public final int getTaskId()
```


タスクに 'Attach to task' オプションが選択されている場合はタスクの Id を取得し、そうでない場合は -1 を返します。

**Returns:**
int - 'Attach to task' オプションが選択された場合のタスク ID、そうでない場合は -1。
### getTimescaleDate() {#getTimescaleDate--}
```
public final Date getTimescaleDate()
```


'Attach to timescale' オプションが選択されている場合のビジュアルオブジェクトの日付配置を取得します。

**Returns:**
java.util.Date - 'Attach to timescale' オプションが選択されたときのビジュアルオブジェクトの日付配置。
### getVerticalOffset() {#getVerticalOffset--}
```
public final double getVerticalOffset()
```


ビジュアルオブジェクトの垂直オフセットを取得します。

**Returns:**
double - ビジュアルオブジェクトの垂直オフセット。
### getWidth() {#getWidth--}
```
public final double getWidth()
```


表示されるビジュアルオブジェクトの幅を取得します。

**Returns:**
double - ビジュアルオブジェクトの表示幅。
### setAttachmentPoint(int value) {#setAttachmentPoint-int-}
```
public final void setAttachmentPoint(int value)
```


'Attach to task' オプションが選択されている場合、タスクに対するビジュアルオブジェクトの配置を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 'Attach to task' オプションが選択されたときのタスクに対するビジュアルオブジェクトの配置。 |

### setBorderLineColor(Color value) {#setBorderLineColor-java.awt.Color-}
```
public final void setBorderLineColor(Color value)
```


境界線の色を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.awt.Color | 境界線の色。 |

### setBorderLineThickness(byte value) {#setBorderLineThickness-byte-}
```
public final void setBorderLineThickness(byte value)
```


境界線の太さを設定します（許容値は0〜5です）。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | バイト | 境界線の太さ（許容値は 0〜5）。 |

### setFillColor(Color value) {#setFillColor-java.awt.Color-}
```
public final void setFillColor(Color value)
```


塗りつぶしの色を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.awt.Color | 塗りつぶし色。 |

### setFillPattern(int value) {#setFillPattern-int-}
```
public final void setFillPattern(int value)
```


塗りつぶしパターンを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 塗りつぶしパターン。 |

### setHeight(double value) {#setHeight-double-}
```
public final void setHeight(double value)
```


表示されるビジュアルオブジェクトの高さを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | double | ビジュアルオブジェクトの表示高さ。 |

### setHorizontalOffset(double value) {#setHorizontalOffset-double-}
```
public final void setHorizontalOffset(double value)
```


ビジュアルオブジェクトの水平オフセットを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | double | ビジュアルオブジェクトの水平オフセット。 |

### setOleObjectId(int value) {#setOleObjectId-int-}
```
public final void setOleObjectId(int value)
```


[OleObject](../../com.aspose.tasks/oleobject) オブジェクトの Id を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | int | [OleObject](../../com.aspose/tasks/oleobject) オブジェクトの ID。 |

### setTaskId(int value) {#setTaskId-int-}
```
public final void setTaskId(int value)
```


'Attach to task' オプションが選択されている場合はタスクの Id を設定し、そうでない場合は -1 を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 'Attach to task' オプションが選択された場合のタスク ID、そうでない場合は -1。 |

### setTimescaleDate(Date value) {#setTimescaleDate-java.util.Date-}
```
public final void setTimescaleDate(Date value)
```


'Attach to timescale' オプションが選択されている場合、ビジュアルオブジェクトの日付配置を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | 'Attach to timescale' オプションが選択されたときのビジュアルオブジェクトの日付配置。 |

### setVerticalOffset(double value) {#setVerticalOffset-double-}
```
public final void setVerticalOffset(double value)
```


ビジュアルオブジェクトの垂直オフセットを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | double | ビジュアルオブジェクトの垂直オフセット。 |

### setWidth(double value) {#setWidth-double-}
```
public final void setWidth(double value)
```


表示されるビジュアルオブジェクトの幅を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | double | ビジュアルオブジェクトの表示幅。 |

