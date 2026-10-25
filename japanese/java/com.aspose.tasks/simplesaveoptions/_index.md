---
title: "SimpleSaveOptions"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "これは、特定の形式でプロジェクトを保存する際にユーザーが基本オプションを指定できる抽象基底クラスです。"
type: docs
weight: 277
url: /ja/java/com.aspose.tasks/simplesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class SimpleSaveOptions
```

これは、特定の形式でプロジェクトを保存する際にユーザーが基本オプションを指定できる抽象基底クラスです。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [SimpleSaveOptions()](#SimpleSaveOptions--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getSaveFormat()](#getSaveFormat--) | この保存オプションオブジェクトが使用される場合に、ドキュメントが保存される形式を取得します。 |
| [getTasksComparer()](#getTasksComparer--) | ガントチャートとタスクシートチャートでタスクを並べ替えるための比較子を取得します。 |
| [getTasksFilter()](#getTasksFilter--) | ガント、タスクシート、タスク使用状況チャートに描画されるタスクをフィルタリングするために使用される条件を取得します。 |
| [setTasksComparer(Comparator&lt;Task&gt; value)](#setTasksComparer-java.util.Comparator-com.aspose.tasks.Task--) | ガントチャートとタスクシートチャートでタスクを並べ替える比較子を設定します。 |
| [setTasksFilter(ICondition&lt;Task&gt; value)](#setTasksFilter-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | ガント、タスクシート、タスク使用状況チャートに描画されるタスクをフィルタリングする条件を設定します。 |
### SimpleSaveOptions() {#SimpleSaveOptions--}
```
public SimpleSaveOptions()
```


### getSaveFormat() {#getSaveFormat--}
```
public final int getSaveFormat()
```


この保存オプションオブジェクトが使用される場合に、ドキュメントが保存される形式を取得します。

**Returns:**
int - ドキュメントが保存される [SaveFileFormat](../../com.aspose.tasks/savefileformat) です。
### getTasksComparer() {#getTasksComparer--}
```
public final Comparator<Task> getTasksComparer()
```


ガントチャートとタスクシートチャートでタスクを並べ替えるための比較子を取得します。

**Returns:**
java.util.Comparator&lt;com.aspose.tasks.Task&gt; - ガントチャートとタスクシートチャートでタスクを並べ替える比較子です。
### getTasksFilter() {#getTasksFilter--}
```
public final ICondition<Task> getTasksFilter()
```


ガント、タスクシート、タスク使用状況チャートに描画されるタスクをフィルタリングするために使用される条件を取得します。

--------------------

値が指定されていない場合、デフォルトのフィルタが使用され、非表示タスク（つまり、折りたたまれたタスクの子タスク）を除外します。

**Returns:**
[ICondition](../../com.aspose.tasks/icondition) - the condition which is used to filter tasks rendered on Gantt, Task Sheet and Task Usage charts.
### setTasksComparer(Comparator&lt;Task&gt; value) {#setTasksComparer-java.util.Comparator-com.aspose.tasks.Task--}
```
public final void setTasksComparer(Comparator<Task> value)
```


ガントチャートとタスクシートチャートでタスクを並べ替える比較子を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Comparator&lt;com.aspose.tasks.Task&gt; | ガントチャートとタスクシートチャートでタスクを並べ替える比較子です。 |

### setTasksFilter(ICondition&lt;Task&gt; value) {#setTasksFilter-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public final void setTasksFilter(ICondition<Task> value)
```


ガント、タスクシート、タスク使用状況チャートに描画されるタスクをフィルタリングする条件を設定します。

--------------------

値が指定されていない場合、デフォルトのフィルタが使用され、非表示タスク（つまり、折りたたまれたタスクの子タスク）を除外します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | ガント、タスクシート、タスク使用状況チャートに描画されるタスクをフィルタリングする条件です。 |

