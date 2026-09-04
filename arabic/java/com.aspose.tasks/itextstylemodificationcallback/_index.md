---
title: "ITextStyleModificationCallback"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل رد نداء يتم استدعاؤه قبل تطبيق TextStyle على خلية جدول."
type: docs
weight: 383
url: /ar/java/com.aspose.tasks/itextstylemodificationcallback/
---
```
public interface ITextStyleModificationCallback
```

يمثل رد نداء يتم استدعاؤه قبل تطبيق TextStyle على خلية جدول.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [beforeTaskTextStyleApplied(TaskTextStyleEventArgs args)](#beforeTaskTextStyleApplied-com.aspose.tasks.TaskTextStyleEventArgs-) | الطريقة التي سيتم استدعاؤها قبل رسم خلية جدول لسطر مهمة في العروض التالية: 'Gantt Chart'، 'Task Sheet'، 'Task Usage'. |
### beforeTaskTextStyleApplied(TaskTextStyleEventArgs args) {#beforeTaskTextStyleApplied-com.aspose.tasks.TaskTextStyleEventArgs-}
```
public abstract void beforeTaskTextStyleApplied(TaskTextStyleEventArgs args)
```


الطريقة التي سيتم استدعاؤها قبل رسم خلية جدول لسطر مهمة في العروض التالية: 'Gantt Chart'، 'Task Sheet'، 'Task Usage'.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| args | [TaskTextStyleEventArgs](../../com.aspose.tasks/tasktextstyleeventargs) | الكائن [TaskTextStyleEventArgs](../../com.aspose.tasks/tasktextstyleeventargs). |

