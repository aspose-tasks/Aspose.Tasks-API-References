---
title: "CheckCircuit"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "タスクのツリーに回路が含まれているかどうかをチェックします。"
type: docs
weight: 48
url: /ja/java/com.aspose.tasks/checkcircuit/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.TreeAlgorithmBase
```
public class CheckCircuit extends TreeAlgorithmBase<Task>
```

タスクのツリーに回路が含まれているかどうかをチェックします。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [CheckCircuit()](#CheckCircuit--) | 新しい [CheckCircuit](../../com.aspose.tasks/checkcircuit) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [alg(Task el, int level)](#alg-com.aspose.tasks.Task-int-) | 指定されたオブジェクトが既に処理されているかどうかを確認します。 |
### CheckCircuit() {#CheckCircuit--}
```
public CheckCircuit()
```


新しい [CheckCircuit](../../com.aspose.tasks/checkcircuit) クラスのインスタンスを初期化します。

### alg(Task el, int level) {#alg-com.aspose.tasks.Task-int-}
```
public void alg(Task el, int level)
```


指定されたオブジェクトが既に処理されているかどうかを確認します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | 処理対象のオブジェクト。 |
| レベル | int | ツリーノードのレベル。 |

