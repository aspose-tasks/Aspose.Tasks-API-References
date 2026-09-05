---
title: "TaskValidationException"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "再計算後にプロジェクトのタスクでエラーが見つかったときにスローされる例外を表します。"
type: docs
weight: 308
url: /ja/java/com.aspose.tasks/taskvalidationexception/
---

**Inheritance:**
java.lang.Object, java.lang.Throwable, java.lang.Exception, java.lang.RuntimeException, com.aspose.ms.System.Exception, com.aspose.ms.System.ApplicationException, [com.aspose.tasks.ValidationException](../../com.aspose.tasks/validationexception), [com.aspose.tasks.RecalculationValidationException](../../com.aspose.tasks/recalculationvalidationexception)
```
public class TaskValidationException extends RecalculationValidationException
```

再計算後にプロジェクトのタスクでエラーが見つかったときにスローされる例外を表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getTask()](#getTask--) | 例外の原因となったタスクを取得します。 |
### getTask() {#getTask--}
```
public final Task getTask()
```


例外の原因となったタスクを取得します。

**Returns:**
[Task](../../com.aspose.tasks/task) - the task which caused the exception.
