---
title: TaskValidationException
second_title: Aspose.Tasks for Java API Reference
description: Represents an exception which is thrown when errors are found in projects tasks after recalculation.
type: docs
weight: 295
url: /java/com.aspose.tasks/taskvalidationexception/
---

**Inheritance:**
java.lang.Object, java.lang.Throwable, java.lang.Exception, java.lang.RuntimeException, [com.aspose.tasks.exceptions.Exception](../../com.aspose.tasks.exceptions/exception), [com.aspose.tasks.exceptions.ApplicationException](../../com.aspose.tasks.exceptions/applicationexception), [com.aspose.tasks.ValidationException](../../com.aspose.tasks/validationexception), [com.aspose.tasks.RecalculationValidationException](../../com.aspose.tasks/recalculationvalidationexception)
```
public class TaskValidationException extends RecalculationValidationException
```

Represents an exception which is thrown when errors are found in project's tasks after recalculation.
## Methods

| Method | Description |
| --- | --- |
| [getTask()](#getTask--) | Gets the task which caused the exception. |
### getTask() {#getTask--}
```
public final Task getTask()
```


Gets the task which caused the exception.

**Returns:**
[Task](../../com.aspose.tasks/task) - the task which caused the exception.
