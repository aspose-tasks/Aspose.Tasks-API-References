---
title: "TaskValidationException"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل استثناءً يُرمى عندما يتم العثور على أخطاء في مهام المشاريع بعد إعادة الحساب."
type: docs
weight: 308
url: /ar/java/com.aspose.tasks/taskvalidationexception/
---

**Inheritance:**
java.lang.Object, java.lang.Throwable, java.lang.Exception, java.lang.RuntimeException, com.aspose.ms.System.Exception, com.aspose.ms.System.ApplicationException, [com.aspose.tasks.ValidationException](../../com.aspose.tasks/validationexception), [com.aspose.tasks.RecalculationValidationException](../../com.aspose.tasks/recalculationvalidationexception)
```
public class TaskValidationException extends RecalculationValidationException
```

يمثل استثناءً يُرمى عندما يتم العثور على أخطاء في مهام المشروع بعد إعادة الحساب.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getTask()](#getTask--) | يحصل على المهمة التي تسببت في الاستثناء. |
### getTask() {#getTask--}
```
public final Task getTask()
```


يحصل على المهمة التي تسببت في الاستثناء.

**Returns:**
[Task](../../com.aspose.tasks/task) - the task which caused the exception.
