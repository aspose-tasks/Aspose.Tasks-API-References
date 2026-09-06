---
title: "ITextStyleModificationCallback"
second_title: "Aspose.Tasks for Java API Referansı"
description: "TextStyle bir tablo hücresine uygulanmadan önce çağrılan bir geri aramayı temsil eder."
type: docs
weight: 383
url: /tr/java/com.aspose.tasks/itextstylemodificationcallback/
---
```
public interface ITextStyleModificationCallback
```

TextStyle bir tablo hücresine uygulanmadan önce çağrılan bir geri aramayı temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [beforeTaskTextStyleApplied(TaskTextStyleEventArgs args)](#beforeTaskTextStyleApplied-com.aspose.tasks.TaskTextStyleEventArgs-) | Tablo hücresinin bir görev satırı için aşağıdaki görünümlerde render edilmeden önce çağrılacak yöntem: 'Gantt Chart', 'Task Sheet', 'Task Usage'. |
### beforeTaskTextStyleApplied(TaskTextStyleEventArgs args) {#beforeTaskTextStyleApplied-com.aspose.tasks.TaskTextStyleEventArgs-}
```
public abstract void beforeTaskTextStyleApplied(TaskTextStyleEventArgs args)
```


Tablo hücresinin bir görev satırı için aşağıdaki görünümlerde render edilmeden önce çağrılacak yöntem: 'Gantt Chart', 'Task Sheet', 'Task Usage'.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| args | [TaskTextStyleEventArgs](../../com.aspose.tasks/tasktextstyleeventargs) | Bu [TaskTextStyleEventArgs](../../com.aspose.tasks/tasktextstyleeventargs) nesnesi. |

