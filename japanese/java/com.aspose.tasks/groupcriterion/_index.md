---
title: "GroupCriterion"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "グループ定義内の基準を表します。"
type: docs
weight: 124
url: /ja/java/com.aspose.tasks/groupcriterion/
---

**Inheritance:**
java.lang.Object
```
public class GroupCriterion
```

グループ定義の基準を表します。GroupCriterion オブジェクトは [GroupCriterionCollection](../../com.aspose.tasks/groupcriterioncollection) コレクションのメンバーです。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [GroupCriterion()](#GroupCriterion--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。 |
| [getAscending()](#getAscending--) | グループ定義で基準として使用されるフィールドが昇順にソートされているかどうかを示す値を取得します。 |
| [getCellColor()](#getCellColor--) | グループ定義で基準として使用されるフィールドのセル背景色を取得します。 |
| [getField()](#getField--) | グループ化されているフィールドを取得します。 |
| [getFont()](#getFont--) | グループ定義の基準のフォントを取得します。 |
| [getFontColor()](#getFontColor--) | グループ定義で基準として使用されるフィールドのフォント色を取得します。 |
| [getGroupInterval()](#getGroupInterval--) | グループ定義で基準として使用されるフィールドの間隔を取得します。 |
| [getGroupOn()](#getGroupOn--) | グループ定義で基準として使用されるフィールドのグループ化タイプを取得します。 |
| [getPattern()](#getPattern--) | グループ定義で基準として使用されるフィールドのセルパターンを取得します。 |
| [getStartAt()](#getStartAt--) | グループ定義で基準として使用されるフィールドの間隔の開始位置を取得します。 |
| [hashCode()](#hashCode--) | 特定の型に対するハッシュ関数として機能します。 |
| [setAscending(boolean value)](#setAscending-boolean-) | グループ定義で基準として使用されるフィールドが昇順にソートされているかどうかを示す値を設定します。 |
| [setCellColor(Color value)](#setCellColor-java.awt.Color-) | グループ定義で基準として使用されるフィールドのセル背景色を設定します。 |
| [setField(int value)](#setField-int-) | グループ化されるフィールドを設定します。 |
| [setFont(FontDescriptor value)](#setFont-com.aspose.tasks.FontDescriptor-) | グループ定義の基準のフォントを設定します。 |
| [setFontColor(Color value)](#setFontColor-java.awt.Color-) | グループ定義で基準として使用されるフィールドのフォント色を設定します。 |
| [setGroupInterval(Object value)](#setGroupInterval-java.lang.Object-) | グループ定義で基準として使用されるフィールドの間隔を設定します。 |
| [setGroupOn(int value)](#setGroupOn-int-) | グループ定義で基準として使用されるフィールドのグループ化タイプを設定します。 |
| [setPattern(int value)](#setPattern-int-) | グループ定義で基準として使用されるフィールドのセルパターンを設定します。 |
| [setStartAt(Object value)](#setStartAt-java.lang.Object-) | グループ定義で基準として使用されるフィールドの間隔の開始位置を設定します。 |
### GroupCriterion() {#GroupCriterion--}
```
public GroupCriterion()
```


### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| obj | java.lang.Object | このインスタンスと比較するオブジェクトです。 |

**Returns:**
boolean - **True** は、o がこのインスタンスと同じ UID 値を持つ GroupCriterion の場合; それ以外の場合は **false**。
### getAscending() {#getAscending--}
```
public final boolean getAscending()
```


グループ定義で基準として使用されるフィールドが昇順でソートされているかどうかを示す値を取得します。フィールドが降順でソートされている場合は False です。

**Returns:**
boolean - グループ定義で基準として使用されるフィールドが昇順でソートされているかどうかを示す値。
### getCellColor() {#getCellColor--}
```
public final Color getCellColor()
```


グループ定義で基準として使用されるフィールドのセル背景色を取得します。

**Returns:**
java.awt.Color - グループ定義で基準として使用されるフィールドのセル背景色。
### getField() {#getField--}
```
public final int getField()
```


グループ化されているフィールドを取得します。

**Returns:**
int - グループ化対象のフィールド。
### getFont() {#getFont--}
```
public final FontDescriptor getFont()
```


グループ定義の基準のフォントを取得します。

**Returns:**
[FontDescriptor](../../com.aspose.tasks/fontdescriptor) - the font for a criterion in a group definition.
### getFontColor() {#getFontColor--}
```
public final Color getFontColor()
```


グループ定義で基準として使用されるフィールドのフォント色を取得します。

**Returns:**
java.awt.Color - グループ定義で基準として使用されるフィールドのフォント色。
### getGroupInterval() {#getGroupInterval--}
```
public final Object getGroupInterval()
```


グループ定義で基準として使用されるフィールドの間隔を取得します。

**Returns:**
java.lang.Object - グループ定義で基準として使用されるフィールドの間隔。
### getGroupOn() {#getGroupOn--}
```
public final int getGroupOn()
```


グループ定義で基準として使用されるフィールドのグループ化タイプを取得します。

**Returns:**
int - グループ定義で基準として使用されるフィールドのグループ化タイプ。
### getPattern() {#getPattern--}
```
public final int getPattern()
```


グループ定義で基準として使用されるフィールドのセルパターンを取得します。

**Returns:**
int - グループ定義で基準として使用されるフィールドのセルパターン。
### getStartAt() {#getStartAt--}
```
public final Object getStartAt()
```


グループ定義で基準として使用されるフィールドの間隔の開始位置を取得します。

**Returns:**
java.lang.Object - グループ定義で基準として使用されるフィールドの間隔の開始位置。
### hashCode() {#hashCode--}
```
public int hashCode()
```


特定の型に対するハッシュ関数として機能します。

**Returns:**
int - 現在のオブジェクトのハッシュコード。
### setAscending(boolean value) {#setAscending-boolean-}
```
public final void setAscending(boolean value)
```


グループ定義で基準として使用されるフィールドが昇順でソートされているかどうかを示す値を設定します。フィールドが降順でソートされている場合は False です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | グループ定義で基準として使用されるフィールドが昇順でソートされているかどうかを示す値。 |

### setCellColor(Color value) {#setCellColor-java.awt.Color-}
```
public final void setCellColor(Color value)
```


グループ定義で基準として使用されるフィールドのセル背景色を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.awt.Color | グループ定義で基準として使用されるフィールドのセル背景色。 |

### setField(int value) {#setField-int-}
```
public final void setField(int value)
```


グループ化されるフィールドを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | グループ化対象のフィールド。 |

### setFont(FontDescriptor value) {#setFont-com.aspose.tasks.FontDescriptor-}
```
public final void setFont(FontDescriptor value)
```


グループ定義の基準のフォントを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | グループ定義で基準となるフィールドのフォント。 |

### setFontColor(Color value) {#setFontColor-java.awt.Color-}
```
public final void setFontColor(Color value)
```


グループ定義で基準として使用されるフィールドのフォント色を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.awt.Color | グループ定義で基準として使用されるフィールドのフォント色。 |

### setGroupInterval(Object value) {#setGroupInterval-java.lang.Object-}
```
public final void setGroupInterval(Object value)
```


グループ定義で基準として使用されるフィールドの間隔を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.Object | グループ定義で基準として使用されるフィールドの間隔。 |

### setGroupOn(int value) {#setGroupOn-int-}
```
public final void setGroupOn(int value)
```


グループ定義で基準として使用されるフィールドのグループ化タイプを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | グループ定義で基準として使用されるフィールドのグループ化タイプ。 |

### setPattern(int value) {#setPattern-int-}
```
public final void setPattern(int value)
```


グループ定義で基準として使用されるフィールドのセルパターンを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | グループ定義で基準として使用されるフィールドのセルパターン。 |

### setStartAt(Object value) {#setStartAt-java.lang.Object-}
```
public final void setStartAt(Object value)
```


グループ定義で基準として使用されるフィールドの間隔の開始位置を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.Object | グループ定義で基準として使用されるフィールドの間隔の開始位置。 |

