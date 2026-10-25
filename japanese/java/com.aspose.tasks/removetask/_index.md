---
title: "RemoveTask"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "指定されたタスクをタスクツリーから削除します。"
type: docs
weight: 246
url: /ja/java/com.aspose.tasks/removetask/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ITreeAlgorithm
```
public class RemoveTask implements ITreeAlgorithm<Task>
```

指定されたタスクをタスクツリーから削除します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [RemoveTask(Task task)](#RemoveTask-com.aspose.tasks.Task-) | 新しいインスタンスを初期化します。[RemoveTask](../../com.aspose.tasks/removetask) クラス。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [alg(Task el, int level)](#alg-com.aspose.tasks.Task-int-) | 何もしません。 |
| [postAlg(Task el, int level)](#postAlg-com.aspose.tasks.Task-int-) | 何もしません。 |
| [preAlg(Task el, int level)](#preAlg-com.aspose.tasks.Task-int-) | 指定された親タスクからタスクを削除します。 |
### RemoveTask(Task task) {#RemoveTask-com.aspose.tasks.Task-}
```
public RemoveTask(Task task)
```


新しいインスタンスを初期化します。[RemoveTask](../../com.aspose.tasks/removetask) クラス。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | 削除するタスク。 |

### alg(Task el, int level) {#alg-com.aspose.tasks.Task-int-}
```
public final void alg(Task el, int level)
```


何もしません。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | 処理対象のオブジェクト。 |
| レベル | int | ツリーノードのレベル。 |

### postAlg(Task el, int level) {#postAlg-com.aspose.tasks.Task-int-}
```
public final void postAlg(Task el, int level)
```


何もしません。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | 処理対象のオブジェクト。 |
| レベル | int | ツリーノードのレベル。 |

### preAlg(Task el, int level) {#preAlg-com.aspose.tasks.Task-int-}
```
public final void preAlg(Task el, int level)
```


指定された親タスクからタスクを削除します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | 親タスク。 |
| レベル | int | ツリーノードのレベル。 |

