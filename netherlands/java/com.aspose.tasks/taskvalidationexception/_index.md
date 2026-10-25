---
title: "TaskValidationException"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een uitzondering voor die wordt gegooid wanneer fouten worden gevonden in projecttaken na herberekening."
type: docs
weight: 308
url: /nl/java/com.aspose.tasks/taskvalidationexception/
---

**Inheritance:**
java.lang.Object, java.lang.Throwable, java.lang.Exception, java.lang.RuntimeException, com.aspose.ms.System.Exception, com.aspose.ms.System.ApplicationException, [com.aspose.tasks.ValidationException](../../com.aspose.tasks/validationexception), [com.aspose.tasks.RecalculationValidationException](../../com.aspose.tasks/recalculationvalidationexception)
```
public class TaskValidationException extends RecalculationValidationException
```

Stelt een uitzondering voor die wordt gegooid wanneer fouten worden gevonden in de taken van het project na herberekening.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getTask()](#getTask--) | Haalt de taak op die de uitzondering veroorzaakte. |
### getTask() {#getTask--}
```
public final Task getTask()
```


Haalt de taak op die de uitzondering veroorzaakte.

**Returns:**
[Task](../../com.aspose.tasks/task) - the task which caused the exception.
