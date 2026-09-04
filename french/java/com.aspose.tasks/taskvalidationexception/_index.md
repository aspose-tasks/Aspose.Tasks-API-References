---
title: "TaskValidationException"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente une exception qui est levée lorsque des erreurs sont trouvées dans les tâches de projets après le recalcul."
type: docs
weight: 308
url: /fr/java/com.aspose.tasks/taskvalidationexception/
---

**Inheritance:**
java.lang.Object, java.lang.Throwable, java.lang.Exception, java.lang.RuntimeException, com.aspose.ms.System.Exception, com.aspose.ms.System.ApplicationException, [com.aspose.tasks.ValidationException](../../com.aspose.tasks/validationexception), [com.aspose.tasks.RecalculationValidationException](../../com.aspose.tasks/recalculationvalidationexception)
```
public class TaskValidationException extends RecalculationValidationException
```

Représente une exception qui est levée lorsque des erreurs sont trouvées dans les tâches du projet après le recalcul.
## Méthodes

| Méthode | Description |
| --- | --- |
| [getTask()](#getTask--) | Obtient la tâche qui a causé l'exception. |
### getTask() {#getTask--}
```
public final Task getTask()
```


Obtient la tâche qui a causé l'exception.

**Returns:**
[Task](../../com.aspose.tasks/task) - the task which caused the exception.
