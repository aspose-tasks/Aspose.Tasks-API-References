---
title: "GanttChartColumn"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "Projects ビュー クラス"
type: docs
weight: 111
url: /ja/java/com.aspose.tasks/ganttchartcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public final class GanttChartColumn extends ViewColumn
```

プロジェクトのビュー クラス
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field)](#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-int-) | GanttChartColumn クラスの新しいインスタンスを初期化します。 |
| [GanttChartColumn(String name, int width, TaskToColumnTextConverter converter)](#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-) | GanttChartColumn クラスの新しいインスタンスを初期化します。 |
| [GanttChartColumn(int width, int field)](#GanttChartColumn-int-int-) | GanttChartColumn クラスの新しいインスタンスを初期化します。 |
| [GanttChartColumn(String name, int width, int field)](#GanttChartColumn-java.lang.String-int-int-) | GanttChartColumn クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getColumnText(Task task)](#getColumnText-com.aspose.tasks.Task-) | 現在のタスクを列テキストに変換します。 |
| [getField()](#getField--) | 列フィールドを返します。 |
| [setField(int value)](#setField-int-) | 列フィールドを設定します。 |
### GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field) {#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-int-}
```
public GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field)
```


GanttChartColumn クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | java.lang.String | 列の名前です。 |
| width | int | 列の幅（ピクセル単位）です。 |
| converter | [TaskToColumnTextConverter](../../com.aspose.tasks/tasktocolumntextconverter) | タスクデータを列テキストに変換するコンバータ。 |
| フィールド | int | 列フィールド。 |

### GanttChartColumn(String name, int width, TaskToColumnTextConverter converter) {#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-}
```
public GanttChartColumn(String name, int width, TaskToColumnTextConverter converter)
```


GanttChartColumn クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | java.lang.String | 列の名前です。 |
| width | int | 列の幅（ピクセル単位）です。 |
| converter | [TaskToColumnTextConverter](../../com.aspose.tasks/tasktocolumntextconverter) | タスクデータを列テキストに変換するコンバータ。 |

### GanttChartColumn(int width, int field) {#GanttChartColumn-int-int-}
```
public GanttChartColumn(int width, int field)
```


GanttChartColumn クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| width | int | 列幅（ピクセル単位）。 |
| フィールド | int | 列フィールド。 |

### GanttChartColumn(String name, int width, int field) {#GanttChartColumn-java.lang.String-int-int-}
```
public GanttChartColumn(String name, int width, int field)
```


GanttChartColumn クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | java.lang.String | 列名。 |
| width | int | 列幅（ピクセル単位）。 |
| フィールド | int | 列フィールド。 |

### getColumnText(Task task) {#getColumnText-com.aspose.tasks.Task-}
```
public final String getColumnText(Task task)
```


現在のタスクを列テキストに変換します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | 現在のタスク。 |

**Returns:**
java.lang.String - 列テキストです。
### getField() {#getField--}
```
public int getField()
```


列フィールドを返します。 `Field`。

**Returns:**
int - 列フィールドの値です。
### setField(int value) {#setField-int-}
```
public void setField(int value)
```


列フィールドを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 列フィールドの値です。 |

