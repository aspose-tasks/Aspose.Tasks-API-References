---
title: "ChildTasksCollector"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "すべての子タスクを収集します。"
type: docs
weight: 49
url: /ja/java/com.aspose.tasks/childtaskscollector/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.TreeAlgorithmBase
```
public class ChildTasksCollector extends TreeAlgorithmBase<Task>
```

すべての子タスクを収集します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [ChildTasksCollector()](#ChildTasksCollector--) | 新しい [ChildTasksCollector](../../com.aspose.tasks/childtaskscollector) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [alg(Task el, int level)](#alg-com.aspose.tasks.Task-int-) | 指定されたオブジェクトを処理します。 |
| [getTasks()](#getTasks--) | 収集された子オブジェクト（タスク）のリストを取得します。 |
### ChildTasksCollector() {#ChildTasksCollector--}
```
public ChildTasksCollector()
```


新しい [ChildTasksCollector](../../com.aspose.tasks/childtaskscollector) クラスのインスタンスを初期化します。

### alg(Task el, int level) {#alg-com.aspose.tasks.Task-int-}
```
public void alg(Task el, int level)
```


指定されたオブジェクトを処理します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | 処理対象のオブジェクト。 |
| レベル | int | ツリーノードのレベル。 |

### getTasks() {#getTasks--}
```
public final List<Task> getTasks()
```


収集された子オブジェクト（タスク）のリストを取得します。

**Returns:**
java.util.List&lt;com.aspose.tasks.Task&gt; - 収集された子オブジェクト（タスク）のリストです。
