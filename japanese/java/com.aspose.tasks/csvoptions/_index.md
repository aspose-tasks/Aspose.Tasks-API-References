---
title: "CsvOptions"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "プロジェクトを CSV に保存する際に追加オプションを指定できるようにします。"
type: docs
weight: 56
url: /ja/java/com.aspose.tasks/csvoptions/
---

**Inheritance:**
java.lang.Object、[com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class CsvOptions extends SimpleSaveOptions
```

プロジェクトを CSV に保存する際に追加オプションを指定できるようにします。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [CsvOptions()](#CsvOptions--) | CSV 形式でプロジェクトを保存するために使用できる [CsvOptions](../../com.aspose/tasks/csvoptions) クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getDataCategory()](#getDataCategory--) | 保存するデータカテゴリを取得します。 |
| [getEncoding()](#getEncoding--) | CSV を保存する際のエンコーディングを取得します。 |
| [getIncludeHeaders()](#getIncludeHeaders--) | ヘッダーを含めるかどうかを示す値を取得します（デフォルト値は TRUE）。 |
| [getTextDelimiter()](#getTextDelimiter--) | テキスト区切り文字を取得します。 |
| [getView()](#getView--) | XLSX 形式で保存するためのビュー列のリスト（[GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)）を取得します。 |
| [setDataCategory(int value)](#setDataCategory-int-) | 保存するデータカテゴリを設定します。 |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | CSV を保存する際のエンコーディングを設定します。 |
| [setIncludeHeaders(boolean value)](#setIncludeHeaders-boolean-) | ヘッダーを含めるかどうかを示す値を設定します（デフォルト値は TRUE）。 |
| [setTextDelimiter(int value)](#setTextDelimiter-int-) | テキスト区切り文字を設定します。 |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | XLSX 形式で保存するためのビュー列のリスト（[GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)）を設定します。 |
### CsvOptions() {#CsvOptions--}
```
public CsvOptions()
```


CSV 形式でプロジェクトを保存するために使用できる [CsvOptions](../../com.aspose/tasks/csvoptions) クラスの新しいインスタンスを初期化します。

### getDataCategory() {#getDataCategory--}
```
public final int getDataCategory()
```


保存するデータカテゴリを取得します。

**Returns:**
int - 保存するデータカテゴリです。
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


CSV を保存する際のエンコーディングを取得します。

**Returns:**
java.nio.charset.Charset - CSV を保存する際のエンコーディングです。
### getIncludeHeaders() {#getIncludeHeaders--}
```
public final boolean getIncludeHeaders()
```


ヘッダーを含めるかどうかを示す値を取得します（デフォルト値は TRUE）。

**Returns:**
boolean - ヘッダーを含めるかどうかを示す値です（デフォルトは TRUE）。
### getTextDelimiter() {#getTextDelimiter--}
```
public final int getTextDelimiter()
```


テキスト区切り文字を取得します。

**Returns:**
int - テキストの区切り文字です。
### getView() {#getView--}
```
public final ProjectView getView()
```


XLSX 形式で保存するためのビュー列のリスト（[GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)）を取得します。設定されていない場合はデフォルト列が保存されます。

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save to XLSX format.
### setDataCategory(int value) {#setDataCategory-int-}
```
public final void setDataCategory(int value)
```


保存するデータカテゴリを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 保存するデータカテゴリです。 |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


CSV を保存する際のエンコーディングを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.nio.charset.Charset | CSV を保存する際のエンコーディングです。 |

### setIncludeHeaders(boolean value) {#setIncludeHeaders-boolean-}
```
public final void setIncludeHeaders(boolean value)
```


ヘッダーを含めるかどうかを示す値を設定します（デフォルト値は TRUE）。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | ヘッダーを含めるかどうかを示す値です（デフォルトは TRUE）。 |

### setTextDelimiter(int value) {#setTextDelimiter-int-}
```
public final void setTextDelimiter(int value)
```


テキスト区切り文字を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | テキストの区切り文字です。 |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


XLSX 形式で保存するためのビュー列のリスト（[GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)）を設定します。設定されていない場合はデフォルト列が保存されます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | XLSX 形式で保存するためのビュー列のリスト（[GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)）です。 |

