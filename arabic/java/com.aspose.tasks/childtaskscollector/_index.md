---
title: "ChildTasksCollector"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يجمع جميع المهام الفرعية."
type: docs
weight: 49
url: /ar/java/com.aspose.tasks/childtaskscollector/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.TreeAlgorithmBase
```
public class ChildTasksCollector extends TreeAlgorithmBase<Task>
```

يجمع جميع المهام الفرعية.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [ChildTasksCollector()](#ChildTasksCollector--) | يُهيئ مثيلاً جديداً للفئة [ChildTasksCollector](../../com.aspose.tasks/childtaskscollector). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [alg(Task el, int level)](#alg-com.aspose.tasks.Task-int-) | يعالج الكائن المحدد. |
| [getTasks()](#getTasks--) | يحصل على قائمة بالكائنات الفرعية المجمعة (المهام). |
### ChildTasksCollector() {#ChildTasksCollector--}
```
public ChildTasksCollector()
```


يُهيئ مثيلاً جديداً للفئة [ChildTasksCollector](../../com.aspose.tasks/childtaskscollector).

### alg(Task el, int level) {#alg-com.aspose.tasks.Task-int-}
```
public void alg(Task el, int level)
```


يعالج الكائن المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | الكائن للمعالجة. |
| المستوى | int | مستوى عقدة الشجرة. |

### getTasks() {#getTasks--}
```
public final List<Task> getTasks()
```


يحصل على قائمة بالكائنات الفرعية المجمعة (المهام).

**Returns:**
java.util.List&lt;com.aspose.tasks.Task&gt; - قائمة بالكائنات الفرعية المجمعة (المهام).
