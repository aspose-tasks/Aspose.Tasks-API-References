---
title: "TaskValidationException"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta un'eccezione che viene sollevata quando vengono trovati errori nelle attività del progetto dopo la ricalcolazione."
type: docs
weight: 308
url: /it/java/com.aspose.tasks/taskvalidationexception/
---

**Inheritance:**
java.lang.Object, java.lang.Throwable, java.lang.Exception, java.lang.RuntimeException, com.aspose.ms.System.Exception, com.aspose.ms.System.ApplicationException, [com.aspose.tasks.ValidationException](../../com.aspose.tasks/validationexception), [com.aspose.tasks.RecalculationValidationException](../../com.aspose.tasks/recalculationvalidationexception)
```
public class TaskValidationException extends RecalculationValidationException
```

Rappresenta un'eccezione che viene lanciata quando vengono trovati errori nelle attività del progetto dopo il ricalcolo.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getTask()](#getTask--) | Restituisce l'attività che ha causato l'eccezione. |
### getTask() {#getTask--}
```
public final Task getTask()
```


Restituisce l'attività che ha causato l'eccezione.

**Returns:**
[Task](../../com.aspose.tasks/task) - the task which caused the exception.
