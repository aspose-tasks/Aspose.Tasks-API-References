---
title: "TaskValidationException"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili pengecualian yang dilemparkan ketika kesalahan ditemukan dalam tugas proyek setelah perhitungan ulang."
type: docs
weight: 308
url: /id/java/com.aspose.tasks/taskvalidationexception/
---

**Inheritance:**
java.lang.Object, java.lang.Throwable, java.lang.Exception, java.lang.RuntimeException, com.aspose.ms.System.Exception, com.aspose.ms.System.ApplicationException, [com.aspose.tasks.ValidationException](../../com.aspose.tasks/validationexception), [com.aspose.tasks.RecalculationValidationException](../../com.aspose.tasks/recalculationvalidationexception)
```
public class TaskValidationException extends RecalculationValidationException
```

Mewakili pengecualian yang dilemparkan ketika kesalahan ditemukan dalam tugas proyek setelah perhitungan ulang.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getTask()](#getTask--) | Mendapatkan tugas yang menyebabkan pengecualian. |
### getTask() {#getTask--}
```
public final Task getTask()
```


Mendapatkan tugas yang menyebabkan pengecualian.

**Returns:**
[Task](../../com.aspose.tasks/task) - the task which caused the exception.
