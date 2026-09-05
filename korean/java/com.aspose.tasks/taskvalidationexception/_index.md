---
title: "TaskValidationException"
second_title: "Aspose.Tasks for Java API Reference"
description: "재계산 후 프로젝트 작업에서 오류가 발견될 때 발생하는 예외를 나타냅니다."
type: docs
weight: 308
url: /ko/java/com.aspose.tasks/taskvalidationexception/
---

**Inheritance:**
java.lang.Object, java.lang.Throwable, java.lang.Exception, java.lang.RuntimeException, com.aspose.ms.System.Exception, com.aspose.ms.System.ApplicationException, [com.aspose.tasks.ValidationException](../../com.aspose.tasks/validationexception), [com.aspose.tasks.RecalculationValidationException](../../com.aspose.tasks/recalculationvalidationexception)
```
public class TaskValidationException extends RecalculationValidationException
```

재계산 후 프로젝트 작업에서 오류가 발견될 때 발생하는 예외를 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getTask()](#getTask--) | 예외를 발생시킨 작업을 가져옵니다. |
### getTask() {#getTask--}
```
public final Task getTask()
```


예외를 발생시킨 작업을 가져옵니다.

**Returns:**
[Task](../../com.aspose.tasks/task) - the task which caused the exception.
