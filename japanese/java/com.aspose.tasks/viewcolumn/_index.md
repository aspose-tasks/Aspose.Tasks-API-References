---
title: "ViewColumn"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "プロジェクトビュー内の列を表します。"
type: docs
weight: 344
url: /ja/java/com.aspose.tasks/viewcolumn/
---

**Inheritance:**
java.lang.Object
```
public abstract class ViewColumn
```

プロジェクトビュー内の列を表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getField()](#getField--) | 列フィールドを取得します。 |
| [getName()](#getName--) | 列名を取得します。 |
| [getStringAlignment()](#getStringAlignment--) | テキストの配置を取得します（[HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment) 列挙体のいずれかの値にできます）。 |
| [getTextStyleModificationCallback()](#getTextStyleModificationCallback--) | 列のセルの外観をカスタマイズするために使用できるコールバックを取得します。 |
| [getWidth()](#getWidth--) | 列の幅を取得します。 |
| [setField(int value)](#setField-int-) | 列フィールドを設定します。 |
| [setStringAlignment(int value)](#setStringAlignment-int-) | テキストの配置を設定します（[HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment) 列挙体のいずれかの値にできます）。 |
| [setTextStyleModificationCallback(ITextStyleModificationCallback value)](#setTextStyleModificationCallback-com.aspose.tasks.ITextStyleModificationCallback-) | 列のセルの外観をカスタマイズするために使用できるコールバックを設定します。 |
### getField() {#getField--}
```
public abstract int getField()
```


列フィールドを取得します。 `Field`([getField()](../../com.aspose.tasks/viewcolumn\#getField--)/[setField(int)](../../com.aspose.tasks/viewcolumn\#setField-int-)).

**Returns:**
int - 列フィールド。
### getName() {#getName--}
```
public final String getName()
```


列名を取得します。

**Returns:**
java.lang.String - 列名。
### getStringAlignment() {#getStringAlignment--}
```
public final int getStringAlignment()
```


テキストの配置を取得します（[HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment) 列挙体のいずれかの値にできます）。

**Returns:**
int - テキストの配置（[HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment) 列挙体のいずれかの値にできます）。
### getTextStyleModificationCallback() {#getTextStyleModificationCallback--}
```
public final ITextStyleModificationCallback getTextStyleModificationCallback()
```


列のセルの外観をカスタマイズするために使用できるコールバックを取得します。

**Returns:**
[ITextStyleModificationCallback](../../com.aspose.tasks/itextstylemodificationcallback) - the callback which can be used to customize the appearance of the column's cells.
### getWidth() {#getWidth--}
```
public final int getWidth()
```


列の幅を取得します。

**Returns:**
int - 列の幅。
### setField(int value) {#setField-int-}
```
public abstract void setField(int value)
```


列フィールドを設定します。 `Field`([getField()](../../com.aspose.tasks/viewcolumn\#getField--)/[setField(int)](../../com.aspose.tasks/viewcolumn\#setField-int-)).

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 列フィールド。 |

### setStringAlignment(int value) {#setStringAlignment-int-}
```
public final void setStringAlignment(int value)
```


テキストの配置を設定します（[HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment) 列挙体のいずれかの値にできます）。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | int | テキストの配置（[HorizontalStringAlignment](../../com.aspose/tasks/horizontalstringalignment) 列挙体の値のいずれかにできます）。 |

### setTextStyleModificationCallback(ITextStyleModificationCallback value) {#setTextStyleModificationCallback-com.aspose.tasks.ITextStyleModificationCallback-}
```
public final void setTextStyleModificationCallback(ITextStyleModificationCallback value)
```


列のセルの外観をカスタマイズするために使用できるコールバックを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [ITextStyleModificationCallback](../../com.aspose.tasks/itextstylemodificationcallback) | 列のセルの外観をカスタマイズするために使用できるコールバック。 |

