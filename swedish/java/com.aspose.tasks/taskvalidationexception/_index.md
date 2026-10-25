---
title: "TaskValidationException"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar ett undantag som kastas när fel hittas i projektuppgifter efter omräkning."
type: docs
weight: 308
url: /sv/java/com.aspose.tasks/taskvalidationexception/
---

**Inheritance:**
java.lang.Object, java.lang.Throwable, java.lang.Exception, java.lang.RuntimeException, com.aspose.ms.System.Exception, com.aspose.ms.System.ApplicationException, [com.aspose.tasks.ValidationException](../../com.aspose.tasks/validationexception), [com.aspose.tasks.RecalculationValidationException](../../com.aspose.tasks/recalculationvalidationexception)
```
public class TaskValidationException extends RecalculationValidationException
```

Representerar ett undantag som kastas när fel hittas i projektets uppgifter efter omräkning.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getTask()](#getTask--) | Hämtar uppgiften som orsakade undantaget. |
### getTask() {#getTask--}
```
public final Task getTask()
```


Hämtar uppgiften som orsakade undantaget.

**Returns:**
[Task](../../com.aspose.tasks/task) - the task which caused the exception.
