---
title: "TimescaleTier"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "ガントチャート上のタイムスケールの単一層を表します。"
type: docs
weight: 325
url: /ja/java/com.aspose.tasks/timescaletier/
---

**Inheritance:**
java.lang.Object
```
public final class TimescaleTier
```

ガントチャート上のタイムスケールの単一層を表します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [TimescaleTier()](#TimescaleTier--) | 新しい [TimescaleTier](../../com.aspose.tasks/timescaletier) クラスのインスタンスを初期化します。 |
| [TimescaleTier(int unit, int count)](#TimescaleTier-int-int-) | 新しい [TimescaleTier](../../com.aspose.tasks/timescaletier) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getAlignment()](#getAlignment--) | ティアの各時間期間内でラベルを揃える方法を取得します（[HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)）。 |
| [getCount()](#getCount--) | ティアのラベルを表示する時間単位間隔を取得します。 |
| [getDateTimeConverter()](#getDateTimeConverter--) | このティアで日付ティックの描画を処理するコールバック関数を取得します。 |
| [getLabel()](#getLabel--) | タイムスケールティアの日時ラベル [DateLabel](../../com.aspose.tasks/datelabel) を取得します。 |
| [getRenderLabelOnEachPage()](#getRenderLabelOnEachPage--) | 時間期間が複数ページにまたがる場合に、各ページに日付ラベルを描画するかどうかを定義するフラグを取得します。 |
| [getShowTicks()](#getShowTicks--) | ティア内で時間期間を区切る目盛りを表示するかどうかを示す値を取得します。 |
| [getUnit()](#getUnit--) | タイムスケールティアのタイムスケール単位 [TimescaleUnit](../../com.aspose.tasks/timescaleunit) を取得します。 |
| [getUsesFiscalYear()](#getUsesFiscalYear--) | ティアラベルを会計年度に基づくかどうかを示す値を取得します。 |
| [setAlignment(int value)](#setAlignment-int-) | ティアの各時間期間内でラベルを揃える方法を設定します（[HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)）。 |
| [setCount(int value)](#setCount-int-) | ティアのラベルを表示する時間単位間隔を設定します。 |
| [setDateTimeConverter(DateTimeConverter value)](#setDateTimeConverter-com.aspose.tasks.DateTimeConverter-) | このティアで日付ティックの描画を処理するコールバック関数を設定します。 |
| [setLabel(int value)](#setLabel-int-) | タイムスケールティアの日時ラベル [DateLabel](../../com.aspose.tasks/datelabel) を設定します。 |
| [setRenderLabelOnEachPage(boolean value)](#setRenderLabelOnEachPage-boolean-) | 時間期間が複数ページにまたがる場合に、各ページに日付ラベルを描画するかどうかを定義するフラグを設定します。 |
| [setShowTicks(boolean value)](#setShowTicks-boolean-) | ティア内で時間期間を区切る目盛りを表示するかどうかを示す値を設定します。 |
| [setUnit(int value)](#setUnit-int-) | タイムスケールティアのタイムスケール単位 [TimescaleUnit](../../com.aspose.tasks/timescaleunit) を設定します。 |
| [setUsesFiscalYear(boolean value)](#setUsesFiscalYear-boolean-) | ティアラベルを会計年度に基づくかどうかを示す値を設定します。 |
### TimescaleTier() {#TimescaleTier--}
```
public TimescaleTier()
```


新しい [TimescaleTier](../../com.aspose.tasks/timescaletier) クラスのインスタンスを初期化します。

### TimescaleTier(int unit, int count) {#TimescaleTier-int-int-}
```
public TimescaleTier(int unit, int count)
```


新しい [TimescaleTier](../../com.aspose.tasks/timescaletier) クラスのインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| unit | int | タイムスケール単位 [TimescaleUnit](../../com.aspose.tasks/timescaleunit)。 |
| count | int | [TimescaleUnit](../../com.aspose.tasks/timescaleunit) 単位の数です。 |

### getAlignment() {#getAlignment--}
```
public final int getAlignment()
```


ティアの各時間期間内でラベルを揃える方法を取得します（[HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)）。

**Returns:**
int - ティアの各時間期間内でラベルを揃える方法（[HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)）。
### getCount() {#getCount--}
```
public final int getCount()
```


ティアのラベルを表示する時間単位間隔を取得します。デフォルト値は 1 です。

**Returns:**
int - ティアのラベルを表示する時間単位間隔。
### getDateTimeConverter() {#getDateTimeConverter--}
```
public final DateTimeConverter getDateTimeConverter()
```


このティアで日付ティックの描画を処理するコールバック関数を取得します。

**Returns:**
[DateTimeConverter](../../com.aspose.tasks/datetimeconverter) - a callback function for handling rendering date tick in this tier.
### getLabel() {#getLabel--}
```
public final int getLabel()
```


タイムスケールティアの日時ラベル [DateLabel](../../com.aspose.tasks/datelabel) を取得します。

**Returns:**
int - タイムスケールティアの日時ラベル [DateLabel](../../com.aspose.tasks/datelabel)。
### getRenderLabelOnEachPage() {#getRenderLabelOnEachPage--}
```
public final boolean getRenderLabelOnEachPage()
```


時間期間が複数ページにまたがる場合に、各ページに日付ラベルを描画するかどうかを定義するフラグを取得します。値が 'true' の場合、期間が複数ページにまたがるとき、期間の日時ラベルは各ページに描画されます。値が 'false' の場合、`Alignment`（[getAlignment](../../com.aspose.tasks/timescaletier\#getAlignment--)/[setAlignment(int)](../../com.aspose.tasks/timescaletier\#setAlignment-int-)) プロパティの値に従って日時ラベルは一度だけ描画されます。

--------------------

MS Project には同等のものがありません。

**Returns:**
boolean - 時間期間が複数ページにまたがる場合に、各ページに日付ラベルを描画するかどうかを定義するフラグ。
### getShowTicks() {#getShowTicks--}
```
public final boolean getShowTicks()
```


ティア内で時間期間を区切る目盛りを表示するかどうかを示す値を取得します。

**Returns:**
boolean - 階層内で時間期間を区切る目盛りを表示するかどうかを示す値。
### getUnit() {#getUnit--}
```
public final int getUnit()
```


タイムスケール階層のタイムスケール単位 [TimescaleUnit](../../com.aspose.tasks/timescaleunit) を取得します。デフォルト値は [TimescaleUnit](../../com.aspose.tasks/timescaleunit) です。

**Returns:**
int - タイムスケール階層のタイムスケール単位 [TimescaleUnit](../../com.aspose.tasks/timescaleunit)。
### getUsesFiscalYear() {#getUsesFiscalYear--}
```
public final boolean getUsesFiscalYear()
```


ティアラベルを会計年度に基づくかどうかを示す値を取得します。

**Returns:**
boolean - 階層ラベルを会計年度に基づくかどうかを示す値。
### setAlignment(int value) {#setAlignment-int-}
```
public final void setAlignment(int value)
```


ティアの各時間期間内でラベルを揃える方法を設定します（[HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)）。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | int | 階層の各時間期間内でラベルをどのように揃えるか ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment))。 |

### setCount(int value) {#setCount-int-}
```
public final void setCount(int value)
```


階層のラベルを表示する時間単位間隔を設定します。デフォルト値は 1 です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 階層のラベルを表示する時間単位間隔。 |

### setDateTimeConverter(DateTimeConverter value) {#setDateTimeConverter-com.aspose.tasks.DateTimeConverter-}
```
public final void setDateTimeConverter(DateTimeConverter value)
```


このティアで日付ティックの描画を処理するコールバック関数を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [DateTimeConverter](../../com.aspose.tasks/datetimeconverter) | この階層で日付目盛りの描画を処理するコールバック関数。 |

### setLabel(int value) {#setLabel-int-}
```
public final void setLabel(int value)
```


タイムスケールティアの日時ラベル [DateLabel](../../com.aspose.tasks/datelabel) を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | int | タイムスケール階層の日時ラベル [DateLabel](../../com.aspose.tasks/datelabel)。 |

### setRenderLabelOnEachPage(boolean value) {#setRenderLabelOnEachPage-boolean-}
```
public final void setRenderLabelOnEachPage(boolean value)
```


時間期間が複数ページにまたがる場合に、各ページに日付ラベルを描画するかどうかを定義するフラグを設定します。値が 'true' の場合、時間期間が複数ページにまたがると、期間の日時ラベルが各ページに描画されます。値が 'false' の場合、`Alignment`([getAlignment](../../com.aspose.tasks/timescaletier\#getAlignment--)/[setAlignment(int)](../../com.aspose.tasks/timescaletier\#setAlignment-int-)) プロパティの値に従って日時ラベルは一度だけ描画されます。

--------------------

MS Project には同等のものがありません。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | 時間期間が複数ページにまたがる場合に、各ページに日付ラベルを描画するかどうかを定義するフラグ。 |

### setShowTicks(boolean value) {#setShowTicks-boolean-}
```
public final void setShowTicks(boolean value)
```


ティア内で時間期間を区切る目盛りを表示するかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | 階層内で時間期間を区切る目盛りを表示するかどうかを示す値。 |

### setUnit(int value) {#setUnit-int-}
```
public final void setUnit(int value)
```


タイムスケール階層のタイムスケール単位 [TimescaleUnit](../../com.aspose.tasks/timescaleunit) を設定します。デフォルト値は [TimescaleUnit](../../com.aspose.tasks/timescaleunit) です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | int | タイムスケール階層のタイムスケール単位 [TimescaleUnit](../../com.aspose.tasks/timescaleunit)。 |

### setUsesFiscalYear(boolean value) {#setUsesFiscalYear-boolean-}
```
public final void setUsesFiscalYear(boolean value)
```


ティアラベルを会計年度に基づくかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | 階層ラベルを会計年度に基づくかどうかを示す値。 |

