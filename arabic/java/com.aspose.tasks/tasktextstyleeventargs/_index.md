---
title: "TaskTextStyleEventArgs"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "هذه الفئة تمثل مجموعة من البيانات المتعلقة بعملية عرض محتوى خلايا الجدول."
type: docs
weight: 302
url: /ar/java/com.aspose.tasks/tasktextstyleeventargs/
---

**Inheritance:**
java.lang.Object
```
public class TaskTextStyleEventArgs
```

تمثل هذه الفئة مجموعة من البيانات المتعلقة بتصيير محتوى خلية الجدول.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getCellTextStyle()](#getCellTextStyle--) | يحصل على TextStyle الذي سيُستخدم لرسم محتوى الخلية. |
| [getColumn()](#getColumn--) | يحصل على [ViewColumn](../../com.aspose.tasks/viewcolumn) التي تنتمي إليها الخلية المعروضة حاليًا. |
| [getTask()](#getTask--) | يحصل على `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) الذي يتطابق مع الصف المعروض حاليًا. |
| [setCellTextStyle(TextStyle value)](#setCellTextStyle-com.aspose.tasks.TextStyle-) | يضبط TextStyle الذي سيُستخدم لرسم محتوى الخلية. |
### getCellTextStyle() {#getCellTextStyle--}
```
public final TextStyle getCellTextStyle()
```


يحصل على TextStyle الذي سيُستخدم لرسم محتوى الخلية. يمكن استخدام هذا الكائن لتخصيص مظهر خلية الجدول.

**Returns:**
[TextStyle](../../com.aspose.tasks/textstyle) - TextStyle which will be used to draw the cell's content.
### getColumn() {#getColumn--}
```
public final ViewColumn getColumn()
```


يحصل على [ViewColumn](../../com.aspose.tasks/viewcolumn) التي تنتمي إليها الخلية المعروضة حاليًا.

**Returns:**
[ViewColumn](../../com.aspose.tasks/viewcolumn) - [ViewColumn](../../com.aspose.tasks/viewcolumn) to which the currently rendered cell belongs.
### getTask() {#getTask--}
```
public final Task getTask()
```


يحصل على `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) الذي يتطابق مع الصف المعروض حاليًا.

**Returns:**
[Task](../../com.aspose.tasks/task) - `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) which corresponds to the currently rendered row.
### setCellTextStyle(TextStyle value) {#setCellTextStyle-com.aspose.tasks.TextStyle-}
```
public final void setCellTextStyle(TextStyle value)
```


يضبط TextStyle الذي سيُستخدم لرسم محتوى الخلية. يمكن استخدام هذا الكائن لتخصيص مظهر خلية الجدول.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [TextStyle](../../com.aspose.tasks/textstyle) | TextStyle الذي سيُستخدم لرسم محتوى الخلية. |

