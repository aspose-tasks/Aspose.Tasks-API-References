---
title: "Table"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "Project のテーブルを表します"
type: docs
weight: 284
url: /ja/java/com.aspose.tasks/table/
---

**Inheritance:**
java.lang.Object
```
public class Table
```

Project のテーブルを表します
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [Table()](#Table--) | 新しい [Table](../../com.aspose.tasks/table) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。 |
| [getAdjustHeaderRowHeight()](#getAdjustHeaderRowHeight--) | テーブルのヘッダー行の高さを調整できるかどうかを示す値を取得します。 |
| [getDateFormat()](#getDateFormat--) | テーブルの日付形式を取得します。 |
| [getLockFirstColumn()](#getLockFirstColumn--) | テーブルの最初の列がロックされているか編集可能かを示す値を取得します。 |
| [getName()](#getName--) | Table オブジェクトの名前を取得します。 |
| [getRowHeight()](#getRowHeight--) | テーブルの行の高さを取得します。行の高さはテキスト行数です。 |
| [getShowAddNewColumn()](#getShowAddNewColumn--) | 'Add New Column' インターフェイスを表示するかどうかを示す値を取得します。 |
| [getShowInMenu()](#getShowInMenu--) | プロジェクトがリボンの表示タブの Tables ドロップダウンリストにテーブル名を表示するかどうかを示す値を取得します。 |
| [getTableFields()](#getTableFields--) | テーブル内のフィールドを表す TableFields コレクションを取得します。 |
| [getTableType()](#getTableType--) | 指定されたテーブルのテーブルタイプを取得します。 |
| [getUid()](#getUid--) | テーブルの一意識別子を取得します。 |
| [hashCode()](#hashCode--) | この Table のハッシュコードを返します。 |
| [setAdjustHeaderRowHeight(boolean value)](#setAdjustHeaderRowHeight-boolean-) | テーブルのヘッダー行の高さを調整できるかどうかを示す値を設定します。 |
| [setDateFormat(int value)](#setDateFormat-int-) | テーブルの日付形式を設定します。 |
| [setLockFirstColumn(boolean value)](#setLockFirstColumn-boolean-) | テーブルの最初の列がロックされているか編集可能かを示す値を設定します。 |
| [setName(String value)](#setName-java.lang.String-) | Table オブジェクトの名前を設定します。 |
| [setRowHeight(int value)](#setRowHeight-int-) | テーブルの行の高さを設定します。行の高さはテキスト行数です。 |
| [setShowAddNewColumn(boolean value)](#setShowAddNewColumn-boolean-) | 'Add New Column' インターフェイスを表示するかどうかを示す値を設定します。 |
| [setShowInMenu(boolean value)](#setShowInMenu-boolean-) | プロジェクトがリボンの表示タブの Tables ドロップダウンリストにテーブル名を表示するかどうかを示す値を設定します。 |
| [setTableType(int value)](#setTableType-int-) | 指定されたテーブルのテーブルタイプを設定します。 |
### Table() {#Table--}
```
public Table()
```


新しい [Table](../../com.aspose.tasks/table) クラスのインスタンスを初期化します。

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
boolean - 指定されたオブジェクトがこのインスタンスと同じ UID 値を持つ Table の場合は **True**、それ以外の場合は **false**。
### getAdjustHeaderRowHeight() {#getAdjustHeaderRowHeight--}
```
public final boolean getAdjustHeaderRowHeight()
```


テーブルのヘッダー行の高さを調整できるかどうかを示す値を取得します。

**Returns:**
boolean - テーブルのヘッダー行の高さを調整できるかどうかを示す値。
### getDateFormat() {#getDateFormat--}
```
public final int getDateFormat()
```


テーブルの日付形式を取得します。

**Returns:**
int - テーブルの日付形式。
### getLockFirstColumn() {#getLockFirstColumn--}
```
public final boolean getLockFirstColumn()
```


テーブルの最初の列がロックされているか編集可能かを示す値を取得します。

**Returns:**
boolean - テーブルの最初の列がロックされているか編集可能かを示す値。
### getName() {#getName--}
```
public final String getName()
```


Table オブジェクトの名前を取得します。

**Returns:**
java.lang.String - Table オブジェクトの名前。
### getRowHeight() {#getRowHeight--}
```
public final int getRowHeight()
```


テーブルの行の高さを取得します。行の高さはテキスト行数です。

**Returns:**
int - テーブルの行の高さ（行の高さはテキスト行数で表されます）。
### getShowAddNewColumn() {#getShowAddNewColumn--}
```
public final boolean getShowAddNewColumn()
```


'Add New Column' インターフェイスを表示するかどうかを示す値を取得します。

--------------------

MSP 2010 バージョン以降でサポートされています。

**Returns:**
boolean - 「Add New Column」インターフェイスを表示するかどうかを示す値。
### getShowInMenu() {#getShowInMenu--}
```
public final boolean getShowInMenu()
```


プロジェクトがリボンの表示タブの Tables ドロップダウンリストにテーブル名を表示するかどうかを示す値を取得します。

**Returns:**
boolean - プロジェクトがリボンの表示タブの Tables ドロップダウンリストにテーブル名を表示するかどうかを示す値。
### getTableFields() {#getTableFields--}
```
public final TableFieldCollection getTableFields()
```


テーブル内のフィールドを表す TableFields コレクションを取得します。

**Returns:**
[TableFieldCollection](../../com.aspose.tasks/tablefieldcollection) - a TableFields collection representing the fields in the table.
### getTableType() {#getTableType--}
```
public final int getTableType()
```


指定されたテーブルのテーブルタイプを取得します。

**Returns:**
int - 指定されたテーブルのテーブルタイプ。
### getUid() {#getUid--}
```
public final int getUid()
```


テーブルの一意識別子を取得します。

**Returns:**
int - テーブルの一意識別子。
### hashCode() {#hashCode--}
```
public int hashCode()
```


この Table のハッシュコードを返します。

**Returns:**
int - このオブジェクトのハッシュコード値を返します。
### setAdjustHeaderRowHeight(boolean value) {#setAdjustHeaderRowHeight-boolean-}
```
public final void setAdjustHeaderRowHeight(boolean value)
```


テーブルのヘッダー行の高さを調整できるかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | テーブルのヘッダー行の高さを調整できるかどうかを示す値。 |

### setDateFormat(int value) {#setDateFormat-int-}
```
public final void setDateFormat(int value)
```


テーブルの日付形式を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | テーブルの日付形式。 |

### setLockFirstColumn(boolean value) {#setLockFirstColumn-boolean-}
```
public final void setLockFirstColumn(boolean value)
```


テーブルの最初の列がロックされているか編集可能かを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | テーブルの最初の列がロックされているか編集可能かを示す値。 |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Table オブジェクトの名前を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | Table オブジェクトの名前。 |

### setRowHeight(int value) {#setRowHeight-int-}
```
public final void setRowHeight(int value)
```


テーブルの行の高さを設定します。行の高さはテキスト行数です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | テーブルの行の高さ（行の高さはテキスト行数で表されます）。 |

### setShowAddNewColumn(boolean value) {#setShowAddNewColumn-boolean-}
```
public final void setShowAddNewColumn(boolean value)
```


'Add New Column' インターフェイスを表示するかどうかを示す値を設定します。

--------------------

MSP 2010 バージョン以降でサポートされています。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | 「Add New Column」インターフェイスを表示するかどうかを示す値。 |

### setShowInMenu(boolean value) {#setShowInMenu-boolean-}
```
public final void setShowInMenu(boolean value)
```


プロジェクトがリボンの表示タブの Tables ドロップダウンリストにテーブル名を表示するかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | プロジェクトがリボンの表示タブの Tables ドロップダウンリストにテーブル名を表示するかどうかを示す値。 |

### setTableType(int value) {#setTableType-int-}
```
public final void setTableType(int value)
```


指定されたテーブルのテーブルタイプを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 指定されたテーブルのテーブルタイプ。 |

