---
title: "TaskValidationException"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt eine Ausnahme dar, die ausgelöst wird, wenn nach der Neuberechnung Fehler in Projektaufgaben gefunden werden."
type: docs
weight: 308
url: /de/java/com.aspose.tasks/taskvalidationexception/
---

**Inheritance:**
java.lang.Object, java.lang.Throwable, java.lang.Exception, java.lang.RuntimeException, com.aspose.ms.System.Exception, com.aspose.ms.System.ApplicationException, [com.aspose.tasks.ValidationException](../../com.aspose.tasks/validationexception), [com.aspose.tasks.RecalculationValidationException](../../com.aspose.tasks/recalculationvalidationexception)
```
public class TaskValidationException extends RecalculationValidationException
```

Stellt eine Ausnahme dar, die ausgelöst wird, wenn nach der Neuberechnung Fehler in den Aufgaben eines Projekts gefunden werden.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getTask()](#getTask--) | Gibt die Aufgabe zurück, die die Ausnahme verursacht hat. |
### getTask() {#getTask--}
```
public final Task getTask()
```


Gibt die Aufgabe zurück, die die Ausnahme verursacht hat.

**Returns:**
[Task](../../com.aspose.tasks/task) - the task which caused the exception.
