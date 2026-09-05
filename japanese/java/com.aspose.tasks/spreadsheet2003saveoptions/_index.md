---
title: "Spreadsheet2003SaveOptions"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "プロジェクトページを Spreadsheet2003 にレンダリングする際に追加オプションを指定できます。"
type: docs
weight: 280
url: /ja/java/com.aspose.tasks/spreadsheet2003saveoptions/
---

**Inheritance:**
java.lang.Object、[com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class Spreadsheet2003SaveOptions extends SimpleSaveOptions
```

プロジェクトページを Spreadsheet2003 にレンダリングする際に追加オプションを指定できます。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [Spreadsheet2003SaveOptions()](#Spreadsheet2003SaveOptions--) | 新しい [Spreadsheet2003SaveOptions](../../com.aspose.tasks/spreadsheet2003saveoptions) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getAssignmentView()](#getAssignmentView--) | レンダリングする割り当てビュー列のリストを取得します ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn))。 |
| [getResourceView()](#getResourceView--) | レンダリングするリソースビュー列のリストを取得します ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn))。 |
| [getView()](#getView--) | 保存するビュー列のリストを取得します ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn))。 |
| [setAssignmentView(ProjectView value)](#setAssignmentView-com.aspose.tasks.ProjectView-) | レンダリングする割り当てビュー列のリストを設定します ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn))。 |
| [setResourceView(ProjectView value)](#setResourceView-com.aspose.tasks.ProjectView-) | レンダリングするリソースビュー列のリストを設定します ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn))。 |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | 保存するビュー列のリストを設定します ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn))。 |
### Spreadsheet2003SaveOptions() {#Spreadsheet2003SaveOptions--}
```
public Spreadsheet2003SaveOptions()
```


新しい [Spreadsheet2003SaveOptions](../../com.aspose.tasks/spreadsheet2003saveoptions) クラスのインスタンスを初期化します。

### getAssignmentView() {#getAssignmentView--}
```
public final ProjectView getAssignmentView()
```


レンダリングする割り当てビュー列のリストを取得します ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn))。

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the assignments view columns to render ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).
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


保存するビュー列のリストを取得します ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn))。設定されていない場合はデフォルト列が保存されます。

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save.
### setAssignmentView(ProjectView value) {#setAssignmentView-com.aspose.tasks.ProjectView-}
```
public final void setAssignmentView(ProjectView value)
```


レンダリングする割り当てビュー列のリストを設定します ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn))。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | レンダリングする割り当てビュー列のリスト ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn))。 |

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


保存するビュー列のリストを設定します ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn))。設定されていない場合はデフォルト列が保存されます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | 保存するビュー列のリスト ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn))。 |

