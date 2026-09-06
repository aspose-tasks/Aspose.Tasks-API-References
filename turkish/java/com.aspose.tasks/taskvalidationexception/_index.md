---
title: "TaskValidationException"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Yeniden hesaplamadan sonra proje görevlerinde hatalar bulunduğunda atılan bir istisna temsil eder."
type: docs
weight: 308
url: /tr/java/com.aspose.tasks/taskvalidationexception/
---

**Inheritance:**
java.lang.Object, java.lang.Throwable, java.lang.Exception, java.lang.RuntimeException, com.aspose.ms.System.Exception, com.aspose.ms.System.ApplicationException, [com.aspose.tasks.ValidationException](../../com.aspose.tasks/validationexception), [com.aspose.tasks.RecalculationValidationException](../../com.aspose.tasks/recalculationvalidationexception)
```
public class TaskValidationException extends RecalculationValidationException
```

Yeniden hesaplamadan sonra projenin görevlerinde hatalar bulunduğunda fırlatılan bir istisnayı temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getTask()](#getTask--) | İstisnaya neden olan görevi alır. |
### getTask() {#getTask--}
```
public final Task getTask()
```


İstisnaya neden olan görevi alır.

**Returns:**
[Task](../../com.aspose.tasks/task) - the task which caused the exception.
