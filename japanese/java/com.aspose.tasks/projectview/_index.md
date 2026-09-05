---
title: "ProjectView"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "Projects ビュー クラス"
type: docs
weight: 228
url: /ja/java/com.aspose.tasks/projectview/
---

**Inheritance:**
java.lang.Object
```
public class ProjectView
```

プロジェクトのビュー クラス
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [ProjectView(Iterable&lt;ViewColumn&gt; columns)](#ProjectView-java.lang.Iterable-com.aspose.tasks.ViewColumn--) | 新しいインスタンスを初期化します [ProjectView](../../com.aspose.tasks/projectview) クラス。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getColumns()](#getColumns--) | プロジェクトビューの列を取得します。 |
| [getDefaultAssignmentView()](#getDefaultAssignmentView--) | Uid、タスク名、リソース名、作業および期間の割り当て列を含みます。 |
| [getDefaultGanttChartView()](#getDefaultGanttChartView--) | id、指標、名前、期間、開始および終了タスク列を含みます。 |
| [getDefaultResourceSheetView()](#getDefaultResourceSheetView--) | Uid、リソース名、タイプ、素材ラベル、イニシャル、グループ、最大単位、標準レート、残業レート、使用ごとのコスト、発生時、基本カレンダー、およびコードリソース列を含みます。 |
| [getDefaultResourceUsageView()](#getDefaultResourceUsageView--) | Uid、名前、開始、終了、および作業リソース列を含みます。 |
| [getDefaultTaskSheetView()](#getDefaultTaskSheetView--) | id、指標、名前、期間、開始、終了、前任タスク、およびリソース名タスク列を含みます。 |
### ProjectView(Iterable&lt;ViewColumn&gt; columns) {#ProjectView-java.lang.Iterable-com.aspose.tasks.ViewColumn--}
```
public ProjectView(Iterable<ViewColumn> columns)
```


新しいインスタンスを初期化します [ProjectView](../../com.aspose.tasks/projectview) クラス。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 列 | java.lang.Iterable&lt;com.aspose.tasks.ViewColumn&gt; | ビュー列のリスト。 |

### getColumns() {#getColumns--}
```
public final List<ViewColumn> getColumns()
```


プロジェクトビューの列を取得します。

**Returns:**
java.util.List&lt;com.aspose.tasks.ViewColumn&gt; - プロジェクトビュー列。
### getDefaultAssignmentView() {#getDefaultAssignmentView--}
```
public static ProjectView getDefaultAssignmentView()
```


Uid、タスク名、リソース名、作業および期間の割り当て列を含みます。

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn).
### getDefaultGanttChartView() {#getDefaultGanttChartView--}
```
public static ProjectView getDefaultGanttChartView()
```


id、指標、名前、期間、開始および終了タスク列を含みます。

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn).
### getDefaultResourceSheetView() {#getDefaultResourceSheetView--}
```
public static ProjectView getDefaultResourceSheetView()
```


Uid、リソース名、タイプ、素材ラベル、イニシャル、グループ、最大単位、標準レート、残業レート、使用ごとのコスト、発生時、基本カレンダー、およびコードリソース列を含みます。

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).
### getDefaultResourceUsageView() {#getDefaultResourceUsageView--}
```
public static ProjectView getDefaultResourceUsageView()
```


Uid、名前、開始、終了、および作業リソース列を含みます。

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).
### getDefaultTaskSheetView() {#getDefaultTaskSheetView--}
```
public static ProjectView getDefaultTaskSheetView()
```


id、指標、名前、期間、開始、終了、前任タスク、およびリソース名タスク列を含みます。

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn).
