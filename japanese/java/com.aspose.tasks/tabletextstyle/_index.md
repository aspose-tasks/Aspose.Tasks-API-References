---
title: "TableTextStyle"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "ビュー テーブル内のテキストスタイルを表します。"
type: docs
weight: 288
url: /ja/java/com.aspose.tasks/tabletextstyle/
---

**Inheritance:**
java.lang.Object、[com.aspose.tasks.TextStyle](../../com.aspose.tasks/textstyle)
```
public class TableTextStyle extends TextStyle
```

ビュー テーブル内のテキストスタイルを表します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [TableTextStyle(int rowUid)](#TableTextStyle-int-) | [TableTextStyle](../../com.aspose.tasks/tabletextstyle) クラスの新しいインスタンスを初期化します。 |
| [TableTextStyle(int rowUid, FontDescriptor font)](#TableTextStyle-int-com.aspose.tasks.FontDescriptor-) | 指定されたフォントを使用して、[TableTextStyle](../../com.aspose.tasks/tabletextstyle) クラスの新しいインスタンスを初期化します。 |
| [TableTextStyle(int rowUid, float fontSize, int fontStyle)](#TableTextStyle-int-float-int-) | 指定されたフォントサイズとフォントスタイルを使用して、[TableTextStyle](../../com.aspose.tasks/tabletextstyle) クラスの新しいインスタンスを初期化します。 |
| [TableTextStyle(int rowUid, int fontStyle)](#TableTextStyle-int-int-) | デフォルトのフォント設定と指定されたフォントスタイルを使用して、[TableTextStyle](../../com.aspose.tasks/tabletextstyle) クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getField()](#getField--) | スタイルが適用されるフィールドを取得します。 |
| [getItemType()](#getItemType--) | テキスト項目のタイプを返します。 |
| [getRowUid()](#getRowUid--) | 行の一意の ID を取得します。 |
| [setField(int value)](#setField-int-) | スタイルが適用されるフィールドを設定します。 |
### TableTextStyle(int rowUid) {#TableTextStyle-int-}
```
public TableTextStyle(int rowUid)
```


[TableTextStyle](../../com.aspose.tasks/tabletextstyle) クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| rowUid | int | 指定された行の一意の ID。 |

### TableTextStyle(int rowUid, FontDescriptor font) {#TableTextStyle-int-com.aspose.tasks.FontDescriptor-}
```
public TableTextStyle(int rowUid, FontDescriptor font)
```


指定されたフォントを使用して、[TableTextStyle](../../com.aspose.tasks/tabletextstyle) クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| rowUid | int | 指定された行の一意の ID。 |
| font | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | テキストスタイルの基になるフォント。 |

### TableTextStyle(int rowUid, float fontSize, int fontStyle) {#TableTextStyle-int-float-int-}
```
public TableTextStyle(int rowUid, float fontSize, int fontStyle)
```


指定されたフォントサイズとフォントスタイルを使用して、[TableTextStyle](../../com.aspose.tasks/tabletextstyle) クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| rowUid | int | 指定された行の一意の ID。 |
| fontSize | float | テキストスタイルの基になるフォントのサイズ。 |
| fontStyle | int | フォントスタイル。 |

### TableTextStyle(int rowUid, int fontStyle) {#TableTextStyle-int-int-}
```
public TableTextStyle(int rowUid, int fontStyle)
```


デフォルトのフォント設定と指定されたフォントスタイルを使用して、[TableTextStyle](../../com.aspose.tasks/tabletextstyle) クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| rowUid | int | 指定された行の一意の ID。 |
| fontStyle | int | フォントスタイル。 |

### getField() {#getField--}
```
public final int getField()
```


スタイルが適用されるフィールドを取得します。 `Field`([getField()](../../com.aspose.tasks/tabletextstyle\#getField--)/[setField(int)](../../com.aspose.tasks/tabletextstyle\#setField-int-)).

**Returns:**
int - スタイルが適用されるフィールド。
### getItemType() {#getItemType--}
```
public int getItemType()
```


テキスト項目のタイプを返します。

**Returns:**
int - TextItemType 列挙型の値。
### getRowUid() {#getRowUid--}
```
public final int getRowUid()
```


行の一意の ID を取得します。

--------------------

ビューのすべての行にスタイルが適用される場合は -1 を返します。

**Returns:**
int - 行の一意の ID。
### setField(int value) {#setField-int-}
```
public final void setField(int value)
```


スタイルが適用されるフィールドを設定します。 `Field`([getField()](../../com.aspose.tasks/tabletextstyle\#getField--)/[setField(int)](../../com.aspose.tasks/tabletextstyle\#setField-int-)).

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | スタイルが適用されるフィールド。 |

