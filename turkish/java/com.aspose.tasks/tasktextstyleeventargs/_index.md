---
title: "TaskTextStyleEventArgs"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Bu sınıf, tablo hücrelerinin içeriğinin işlenmesiyle ilgili veri kümesini temsil eder."
type: docs
weight: 302
url: /tr/java/com.aspose.tasks/tasktextstyleeventargs/
---

**Inheritance:**
java.lang.Object
```
public class TaskTextStyleEventArgs
```

Bu sınıf, tablo hücresinin içeriğinin render edilmesiyle ilgili veri kümesini temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getCellTextStyle()](#getCellTextStyle--) | Hücre içeriğini çizmeye kullanılacak TextStyle'ı alır. |
| [getColumn()](#getColumn--) | Şu anda işlenen hücrenin ait olduğu [ViewColumn](../../com.aspose.tasks/viewcolumn) öğesini alır. |
| [getTask()](#getTask--) | Mevcut işlenen satıra karşılık gelen `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) değerini alır. |
| [setCellTextStyle(TextStyle value)](#setCellTextStyle-com.aspose.tasks.TextStyle-) | Hücre içeriğini çizmeye kullanılacak TextStyle'ı ayarlar. |
### getCellTextStyle() {#getCellTextStyle--}
```
public final TextStyle getCellTextStyle()
```


Hücre içeriğini çizmeye kullanılacak TextStyle'ı alır. Bu nesne bir tablo hücresinin görünümünü özelleştirmek için kullanılabilir.

**Returns:**
[TextStyle](../../com.aspose.tasks/textstyle) - TextStyle which will be used to draw the cell's content.
### getColumn() {#getColumn--}
```
public final ViewColumn getColumn()
```


Şu anda işlenen hücrenin ait olduğu [ViewColumn](../../com.aspose.tasks/viewcolumn) öğesini alır.

**Returns:**
[ViewColumn](../../com.aspose.tasks/viewcolumn) - [ViewColumn](../../com.aspose.tasks/viewcolumn) to which the currently rendered cell belongs.
### getTask() {#getTask--}
```
public final Task getTask()
```


Mevcut işlenen satıra karşılık gelen `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) değerini alır.

**Returns:**
[Task](../../com.aspose.tasks/task) - `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) which corresponds to the currently rendered row.
### setCellTextStyle(TextStyle value) {#setCellTextStyle-com.aspose.tasks.TextStyle-}
```
public final void setCellTextStyle(TextStyle value)
```


Hücre içeriğini çizmeye kullanılacak TextStyle'ı ayarlar. Bu nesne bir tablo hücresinin görünümünü özelleştirmek için kullanılabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [TextStyle](../../com.aspose.tasks/textstyle) | Hücre içeriğini çizmeye kullanılacak TextStyle. |

