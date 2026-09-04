---
title: "TaskUtils"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "فئة مساعدة توفر عمليات مفيدة مع المهام."
type: docs
weight: 307
url: /ar/java/com.aspose.tasks/taskutils/
---

**Inheritance:**
java.lang.Object
```
public class TaskUtils
```

فئة مساعدة توفر عمليات مفيدة مع المهام.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [TaskUtils()](#TaskUtils--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [apply(Task root, ITreeAlgorithm&lt;Task&gt; alg, int level)](#apply-com.aspose.tasks.Task-com.aspose.tasks.ITreeAlgorithm-com.aspose.tasks.Task--int-) | يطبق الخوارزمية المحددة على كل مهمة في شجرة. |
| [filter(Task root, ICondition&lt;Task&gt; cond)](#filter-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | يبني شجرة جديدة من المهام التي تفي بالشرط. |
| [find(Task root, ICondition&lt;Task&gt; cond)](#find-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | يبحث عن مهمة تفي بالشرط في شجرة من المهام. |
| [taskChildrenCount(Task task)](#taskChildrenCount-com.aspose.tasks.Task-) | يحسب بشكل متكرر عدد مهام الأطفال للمهمة عبر جميع المستويات. |
### TaskUtils() {#TaskUtils--}
```
public TaskUtils()
```


### apply(Task root, ITreeAlgorithm&lt;Task&gt; alg, int level) {#apply-com.aspose.tasks.Task-com.aspose.tasks.ITreeAlgorithm-com.aspose.tasks.Task--int-}
```
public static void apply(Task root, ITreeAlgorithm<Task> alg, int level)
```


يطبق الخوارزمية المحددة على كل مهمة في شجرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | جذر الشجرة |
| alg | com.aspose.tasks.ITreeAlgorithm&lt;com.aspose.tasks.Task&gt; | الخوارزمية المطبقة. |
| المستوى | int | مستوى مهمة الجذر. |

### filter(Task root, ICondition&lt;Task&gt; cond) {#filter-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public static Task filter(Task root, ICondition<Task> cond)
```


يبني شجرة جديدة من المهام التي تفي بالشرط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | جذر الشجرة. |
| cond | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | الشرط المطبق. |

**Returns:**
[Task](../../com.aspose.tasks/task) - Root of a new tree.
### find(Task root, ICondition&lt;Task&gt; cond) {#find-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public static Task find(Task root, ICondition<Task> cond)
```


يبحث عن مهمة تفي بالشرط في شجرة من المهام.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | جذر الشجرة. |
| cond | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | الشرط المطبق. |

**Returns:**
[Task](../../com.aspose.tasks/task) - Task if task was found, otherwise null.
### taskChildrenCount(Task task) {#taskChildrenCount-com.aspose.tasks.Task-}
```
public static int taskChildrenCount(Task task)
```


يحسب بشكل متكرر عدد مهام الأطفال للمهمة عبر جميع المستويات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | المهمة التي يتم حساب أطفالها. |

**Returns:**
int - عدد الأطفال.
