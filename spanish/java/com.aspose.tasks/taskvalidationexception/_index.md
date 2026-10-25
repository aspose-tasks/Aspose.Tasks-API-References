---
title: "TaskValidationException"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa una excepción que se lanza cuando se encuentran errores en las tareas de los proyectos después de la recalculación."
type: docs
weight: 308
url: /es/java/com.aspose.tasks/taskvalidationexception/
---

**Inheritance:**
java.lang.Object, java.lang.Throwable, java.lang.Exception, java.lang.RuntimeException, com.aspose.ms.System.Exception, com.aspose.ms.System.ApplicationException, [com.aspose.tasks.ValidationException](../../com.aspose.tasks/validationexception), [com.aspose.tasks.RecalculationValidationException](../../com.aspose.tasks/recalculationvalidationexception)
```
public class TaskValidationException extends RecalculationValidationException
```

Representa una excepción que se lanza cuando se encuentran errores en las tareas del proyecto después de la recalculación.
## Métodos

| Método | Descripción |
| --- | --- |
| [getTask()](#getTask--) | Obtiene la tarea que causó la excepción. |
### getTask() {#getTask--}
```
public final Task getTask()
```


Obtiene la tarea que causó la excepción.

**Returns:**
[Task](../../com.aspose.tasks/task) - the task which caused the exception.
