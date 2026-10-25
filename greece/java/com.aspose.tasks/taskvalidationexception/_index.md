---
title: "TaskValidationException"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αντιπροσωπεύει μια εξαίρεση που ρίχνεται όταν εντοπίζονται σφάλματα στις εργασίες των έργων μετά την επανυπολογισμό."
type: docs
weight: 308
url: /el/java/com.aspose.tasks/taskvalidationexception/
---

**Inheritance:**
java.lang.Object, java.lang.Throwable, java.lang.Exception, java.lang.RuntimeException, com.aspose.ms.System.Exception, com.aspose.ms.System.ApplicationException, [com.aspose.tasks.ValidationException](../../com.aspose.tasks/validationexception), [com.aspose.tasks.RecalculationValidationException](../../com.aspose.tasks/recalculationvalidationexception)
```
public class TaskValidationException extends RecalculationValidationException
```

Αναπαριστά μια εξαίρεση που ρίχνεται όταν εντοπίζονται σφάλματα στις εργασίες του έργου μετά από επανυπολογισμό.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getTask()](#getTask--) | Λαμβάνει την εργασία που προκάλεσε την εξαίρεση. |
### getTask() {#getTask--}
```
public final Task getTask()
```


Λαμβάνει την εργασία που προκάλεσε την εξαίρεση.

**Returns:**
[Task](../../com.aspose.tasks/task) - the task which caused the exception.
