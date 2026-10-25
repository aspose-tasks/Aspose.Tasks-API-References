---
title: "XlsxOptions"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "プロジェクトページを XLSX にレンダリングする際の追加オプションを指定できます。"
type: docs
weight: 368
url: /ja/java/com.aspose.tasks/xlsxoptions/
---

**Inheritance:**
java.lang.Object、[com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class XlsxOptions extends SimpleSaveOptions
```

プロジェクトページを XLSX にレンダリングする際の追加オプションを指定できます。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [XlsxOptions()](#XlsxOptions--) | 新しい [XlsxOptions](../../com.aspose.tasks/xlsxoptions) クラスのインスタンスを初期化します。このクラスはプロジェクトを XLSX 形式で保存するために使用できます。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getAssignmentView()](#getAssignmentView--) | レンダリングする割り当てビュー列のリストを取得します ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn))。 |
| [getEncoding()](#getEncoding--) | 生成された XLSX ファイルのエンコーディングを取得します。 |
| [getResourceView()](#getResourceView--) | レンダリングするリソースビュー列のリストを取得します ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn))。 |
| [getView()](#getView--) | XLSX 形式で保存するためのビュー列のリスト（[GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)）を取得します。 |
| [setAssignmentView(ProjectView value)](#setAssignmentView-com.aspose.tasks.ProjectView-) | レンダリングする割り当てビュー列のリストを設定します ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn))。 |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | 生成された XLSX ファイルのエンコーディングを設定します。 |
| [setResourceView(ProjectView value)](#setResourceView-com.aspose.tasks.ProjectView-) | レンダリングするリソースビュー列のリストを設定します ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn))。 |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | XLSX 形式で保存するためのビュー列のリスト（[GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)）を設定します。 |
### XlsxOptions() {#XlsxOptions--}
```
public XlsxOptions()
```


新しい [XlsxOptions](../../com.aspose.tasks/xlsxoptions) クラスのインスタンスを初期化します。このクラスはプロジェクトを XLSX 形式で保存するために使用できます。

### getAssignmentView() {#getAssignmentView--}
```
public final ProjectView getAssignmentView()
```


レンダリングする割り当てビュー列のリストを取得します ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn))。

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the assignments view columns to render ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


生成された XLSX ファイルのエンコーディングを取得します。デフォルト値は java.nio.charset.StandardCharsets\#UTF\_8.UTF\_8 です。

**Returns:**
java.nio.charset.Charset - 生成された XLSX ファイルのエンコーディング。
### getResourceView() {#getResourceView--}
```
public final ProjectView getResourceView()
```


レンダリングするリソースビュー列のリストを取得します ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn))。

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the resource view columns to render ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).
### getView() {#getView--}
```
public final ProjectView getView()
```


XLSX 形式で保存するためのビュー列のリスト（[GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)）を取得します。設定されていない場合はデフォルト列が保存されます。

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save to XLSX format.
### setAssignmentView(ProjectView value) {#setAssignmentView-com.aspose.tasks.ProjectView-}
```
public final void setAssignmentView(ProjectView value)
```


レンダリングする割り当てビュー列のリストを設定します ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn))。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | レンダリングする割り当てビュー列のリスト ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn))。 |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


生成された XLSX ファイルのエンコーディングを設定します。デフォルト値は java.nio.charset.StandardCharsets\#UTF\_8.UTF\_8 です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.nio.charset.Charset | 生成された XLSX ファイルのエンコーディング。 |

### setResourceView(ProjectView value) {#setResourceView-com.aspose.tasks.ProjectView-}
```
public final void setResourceView(ProjectView value)
```


レンダリングするリソースビュー列のリストを設定します ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn))。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | レンダリングするリソースビュー列のリスト ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn))。 |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


XLSX 形式で保存するためのビュー列のリスト（[GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)）を設定します。設定されていない場合はデフォルト列が保存されます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | XLSX 形式で保存するためのビュー列のリスト（[GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)）です。 |

