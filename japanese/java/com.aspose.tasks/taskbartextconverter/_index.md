---
title: "TaskBarTextConverter"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "タスクデータをバー テキストに変換するカスタムコンバータです。"
type: docs
weight: 290
url: /ja/java/com.aspose.tasks/taskbartextconverter/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.Delegate, com.aspose.ms.System.MulticastDelegate
```
public abstract class TaskBarTextConverter extends System.MulticastDelegate
```

タスクのデータをバーのテキストに変換するカスタムコンバータです。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [TaskBarTextConverter()](#TaskBarTextConverter--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [invoke(Task task)](#invoke-com.aspose.tasks.Task-) | タスクのデータをバーのテキストに変換するカスタムコンバータです。 |
### TaskBarTextConverter() {#TaskBarTextConverter--}
```
public TaskBarTextConverter()
```


### invoke(Task task) {#invoke-com.aspose.tasks.Task-}
```
public abstract String invoke(Task task)
```


タスクのデータをバーのテキストに変換するカスタムコンバータです。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | タスクバーのテキストがレンダリングされるタスクです。 |

**Returns:**
java.lang.String - 指定されたタスクに対応するバーにレンダリングするテキストです。
