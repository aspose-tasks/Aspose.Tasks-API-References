---
title: "OleObject"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "MPP ファイルのガント チャート ビューに挿入できる OLE オブジェクトを表します。"
type: docs
weight: 164
url: /ja/java/com.aspose.tasks/oleobject/
---

**Inheritance:**
java.lang.Object
```
public class OleObject
```

MPP ファイルのガント チャート ビューに挿入できる OLE オブジェクトを表します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [OleObject()](#OleObject--) | 新しい [OleObject](../../com.aspose.tasks/oleobject) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getApplicationName()](#getApplicationName--) | 埋め込みオブジェクトを開くためのアプリケーション名を取得します。 |
| [getContent()](#getContent--) | 埋め込みファイルのデータを取得します。データが埋め込まれていない場合は null です。 |
| [getDisplayAsIcon()](#getDisplayAsIcon--) | OLE オブジェクトをアイコンとして表示するか、通常の画像として表示するかを示すフラグを取得します。 |
| [getFileFormat()](#getFileFormat--) | 埋め込みオブジェクトのファイル形式を取得します。 |
| [getFullPath()](#getFullPath--) | 挿入されたオブジェクトのフルパスを取得します。 |
| [getId()](#getId--) | オブジェクト ID を取得します。 |
| [getLabel()](#getLabel--) | 挿入されたオブジェクトのラベルを取得します。 |
| [getLinked()](#getLinked--) | プロジェクトファイルがリンク元に保存されている実際のデータへのリンクのみを含むかどうかを示す値を取得します。 |
| [getName()](#getName--) | OLE オブジェクトのインスタンス名を取得します。 |
| [getTemporaryFile()](#getTemporaryFile--) | 挿入されたオブジェクトの一時ファイルへのパスを取得します。 |
| [getView()](#getView--) | 挿入されたオブジェクトが属する `View`([getView()](../../com.aspose.tasks/oleobject\#getView--)/[setView(View)](../../com.aspose.tasks/oleobject\#setView-View-)) クラスのインスタンスを取得します。 |
| [setApplicationName(String value)](#setApplicationName-java.lang.String-) | 埋め込みオブジェクトを開くためのアプリケーション名を設定します。 |
| [setContent(byte[] value)](#setContent-byte---) | 埋め込みファイルのデータを設定します。データが埋め込まれていない場合は null です。 |
| [setDisplayAsIcon(boolean value)](#setDisplayAsIcon-boolean-) | OLE オブジェクトをアイコンとして表示するか、通常の画像として表示するかを示すフラグを設定します。 |
| [setFileFormat(String value)](#setFileFormat-java.lang.String-) | 埋め込みオブジェクトのファイル形式を設定します。 |
| [setFullPath(String value)](#setFullPath-java.lang.String-) | 挿入されたオブジェクトのフルパスを設定します。 |
| [setId(int value)](#setId-int-) | オブジェクト ID を設定します。 |
| [setLabel(String value)](#setLabel-java.lang.String-) | 挿入されたオブジェクトのラベルを設定します。 |
| [setName(String value)](#setName-java.lang.String-) | OLE オブジェクトのインスタンス名を設定します。 |
| [setTemporaryFile(String value)](#setTemporaryFile-java.lang.String-) | 挿入されたオブジェクトの一時ファイルへのパスを設定します。 |
| [setView(View value)](#setView-com.aspose.tasks.View-) | 挿入されたオブジェクトが属する `View`([getView()](../../com.aspose.tasks/oleobject\#getView--)/[setView(View)](../../com.aspose.tasks/oleobject\#setView-View-)) クラスのインスタンスを設定します。 |
### OleObject() {#OleObject--}
```
public OleObject()
```


新しい [OleObject](../../com.aspose.tasks/oleobject) クラスのインスタンスを初期化します。

### getApplicationName() {#getApplicationName--}
```
public final String getApplicationName()
```


埋め込みオブジェクトを開くためのアプリケーション名を取得します。

**Returns:**
java.lang.String - 埋め込みオブジェクトを開くためのアプリケーション名。
### getContent() {#getContent--}
```
public final byte[] getContent()
```


埋め込みファイルのデータを取得します。データが埋め込まれていない場合は null です。

**Returns:**
byte[] - 埋め込みファイルのデータ; データが埋め込まれていない場合は null。
### getDisplayAsIcon() {#getDisplayAsIcon--}
```
public final boolean getDisplayAsIcon()
```


OLE オブジェクトをアイコンとして表示するか、通常の画像として表示するかを示すフラグを取得します。

**Returns:**
boolean - OLE オブジェクトをアイコンとして表示するか、通常の画像として表示するかを示すフラグ。
### getFileFormat() {#getFileFormat--}
```
public final String getFileFormat()
```


埋め込みオブジェクトのファイル形式を取得します。

**Returns:**
java.lang.String - 埋め込みオブジェクトのファイル形式。
### getFullPath() {#getFullPath--}
```
public final String getFullPath()
```


挿入されたオブジェクトのフルパスを取得します。

**Returns:**
java.lang.String - 挿入されたオブジェクトのフルパス。
### getId() {#getId--}
```
public final int getId()
```


オブジェクト ID を取得します。

**Returns:**
int - オブジェクト ID。
### getLabel() {#getLabel--}
```
public final String getLabel()
```


挿入されたオブジェクトのラベルを取得します。

**Returns:**
java.lang.String - 挿入されたオブジェクトのラベルです。
### getLinked() {#getLinked--}
```
public final boolean getLinked()
```


プロジェクトファイルがリンク元に保存されている実際のデータへのリンクのみを含むかどうかを示す値を取得します。

**Returns:**
boolean - プロジェクト ファイルがリンク元に保存されている実際のデータへのリンクのみを含むかどうかを示す値です。
### getName() {#getName--}
```
public final String getName()
```


OLE オブジェクトのインスタンス名を取得します。

**Returns:**
java.lang.String - OLE オブジェクトのインスタンス名です。
### getTemporaryFile() {#getTemporaryFile--}
```
public final String getTemporaryFile()
```


挿入されたオブジェクトの一時ファイルへのパスを取得します。

**Returns:**
java.lang.String - 挿入されたオブジェクトの一時ファイルへのパスです。
### getView() {#getView--}
```
public final View getView()
```


挿入されたオブジェクトが属する `View`([getView()](../../com.aspose.tasks/oleobject\#getView--)/[setView(View)](../../com.aspose.tasks/oleobject\#setView-View-)) クラスのインスタンスを取得します。

**Returns:**
[View](../../com.aspose.tasks/view) - the instance of the `View`([getView()](../../com.aspose.tasks/oleobject\#getView--)/[setView(View)](../../com.aspose.tasks/oleobject\#setView-View-)) class the inserted object belongs to.
### setApplicationName(String value) {#setApplicationName-java.lang.String-}
```
public final void setApplicationName(String value)
```


埋め込みオブジェクトを開くためのアプリケーション名を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | 埋め込みオブジェクトを開くためのアプリケーション名です。 |

### setContent(byte[] value) {#setContent-byte---}
```
public final void setContent(byte[] value)
```


埋め込みファイルのデータを設定します。データが埋め込まれていない場合は null です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | byte[] | 埋め込みファイルのデータです。データが埋め込まれていない場合は null です。 |

### setDisplayAsIcon(boolean value) {#setDisplayAsIcon-boolean-}
```
public final void setDisplayAsIcon(boolean value)
```


OLE オブジェクトをアイコンとして表示するか、通常の画像として表示するかを示すフラグを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | OLE オブジェクトをアイコンとして表示するか、通常の画像として表示するかを示すフラグです。 |

### setFileFormat(String value) {#setFileFormat-java.lang.String-}
```
public final void setFileFormat(String value)
```


埋め込みオブジェクトのファイル形式を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | 埋め込みオブジェクトのファイル形式です。 |

### setFullPath(String value) {#setFullPath-java.lang.String-}
```
public final void setFullPath(String value)
```


挿入されたオブジェクトのフルパスを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | 挿入されたオブジェクトのフルパスです。 |

### setId(int value) {#setId-int-}
```
public final void setId(int value)
```


オブジェクト ID を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | オブジェクト ID です。 |

### setLabel(String value) {#setLabel-java.lang.String-}
```
public final void setLabel(String value)
```


挿入されたオブジェクトのラベルを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | 挿入されたオブジェクトのラベルです。 |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


OLE オブジェクトのインスタンス名を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | OLE オブジェクトのインスタンス名です。 |

### setTemporaryFile(String value) {#setTemporaryFile-java.lang.String-}
```
public final void setTemporaryFile(String value)
```


挿入されたオブジェクトの一時ファイルへのパスを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | 挿入されたオブジェクトの一時ファイルへのパスです。 |

### setView(View value) {#setView-com.aspose.tasks.View-}
```
public final void setView(View value)
```


挿入されたオブジェクトが属する `View`([getView()](../../com.aspose.tasks/oleobject\#getView--)/[setView(View)](../../com.aspose.tasks/oleobject\#setView-View-)) クラスのインスタンスを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [View](../../com.aspose.tasks/view) | 挿入されたオブジェクトが属する `View` クラスのインスタンスです。([getView()](../../com.aspose.tasks/oleobject\#getView--)/[setView(View)](../../com.aspose.tasks/oleobject\#setView-View-)) |

