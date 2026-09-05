---
title: "TaskUtils"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "タスクに対して便利な操作を提供するヘルパークラスです。"
type: docs
weight: 307
url: /ja/java/com.aspose.tasks/taskutils/
---

**Inheritance:**
java.lang.Object
```
public class TaskUtils
```

タスクに対して便利な操作を提供するヘルパークラスです。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [TaskUtils()](#TaskUtils--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [apply(Task root, ITreeAlgorithm&lt;Task&gt; alg, int level)](#apply-com.aspose.tasks.Task-com.aspose.tasks.ITreeAlgorithm-com.aspose.tasks.Task--int-) | 指定されたアルゴリズムをツリー内の各タスクに適用します。 |
| [filter(Task root, ICondition&lt;Task&gt; cond)](#filter-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | 条件を満たすタスクの新しいツリーを構築します。 |
| [find(Task root, ICondition&lt;Task&gt; cond)](#find-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | タスクのツリー内で条件を満たすタスクを検索します。 |
| [taskChildrenCount(Task task)](#taskChildrenCount-com.aspose.tasks.Task-) | すべてのレベルにわたって再帰的にタスクの子タスク数を計算します。 |
### TaskUtils() {#TaskUtils--}
```
public TaskUtils()
```


### apply(Task root, ITreeAlgorithm&lt;Task&gt; alg, int level) {#apply-com.aspose.tasks.Task-com.aspose.tasks.ITreeAlgorithm-com.aspose.tasks.Task--int-}
```
public static void apply(Task root, ITreeAlgorithm<Task> alg, int level)
```


指定されたアルゴリズムをツリー内の各タスクに適用します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | ツリーのルート |
| alg | com.aspose.tasks.ITreeAlgorithm&lt;com.aspose.tasks.Task&gt; | 適用されたアルゴリズム。 |
| レベル | int | ルートタスクのレベル。 |

### filter(Task root, ICondition&lt;Task&gt; cond) {#filter-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public static Task filter(Task root, ICondition<Task> cond)
```


条件を満たすタスクの新しいツリーを構築します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | ツリーのルート。 |
| cond | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | 適用された条件。 |

**Returns:**
[Task](../../com.aspose.tasks/task) - Root of a new tree.
### find(Task root, ICondition&lt;Task&gt; cond) {#find-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public static Task find(Task root, ICondition<Task> cond)
```


タスクのツリー内で条件を満たすタスクを検索します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | ツリーのルート。 |
| cond | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | 適用された条件。 |

**Returns:**
[Task](../../com.aspose.tasks/task) - Task if task was found, otherwise null.
### taskChildrenCount(Task task) {#taskChildrenCount-com.aspose.tasks.Task-}
```
public static int taskChildrenCount(Task task)
```


すべてのレベルにわたって再帰的にタスクの子タスク数を計算します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | 子タスクを計算するタスク。 |

**Returns:**
int - 子の数。
