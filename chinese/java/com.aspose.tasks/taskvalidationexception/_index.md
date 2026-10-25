---
title: "TaskValidationException"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示在重新计算后发现项目任务错误时抛出的异常。"
type: docs
weight: 308
url: /zh/java/com.aspose.tasks/taskvalidationexception/
---

**Inheritance:**
java.lang.Object, java.lang.Throwable, java.lang.Exception, java.lang.RuntimeException, com.aspose.ms.System.Exception, com.aspose.ms.System.ApplicationException, [com.aspose.tasks.ValidationException](../../com.aspose.tasks/validationexception), [com.aspose.tasks.RecalculationValidationException](../../com.aspose.tasks/recalculationvalidationexception)
```
public class TaskValidationException extends RecalculationValidationException
```

表示在重新计算后发现项目任务错误时抛出的异常。
## 方法

| 方法 | 描述 |
| --- | --- |
| [getTask()](#getTask--) | 获取导致异常的任务。 |
### getTask() {#getTask--}
```
public final Task getTask()
```


获取导致异常的任务。

**Returns:**
[Task](../../com.aspose.tasks/task) - the task which caused the exception.
