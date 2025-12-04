---
title: TaskUtils
second_title: Aspose.Tasks for Java API Reference
description: Helper class which provides useful operations with tasks.
type: docs
weight: 304
url: /java/com.aspose.tasks/taskutils/
---

**Inheritance:**
java.lang.Object
```
public class TaskUtils
```

Helper class which provides useful operations with tasks.
## Constructors

| Constructor | Description |
| --- | --- |
| [TaskUtils()](#TaskUtils--) |  |
## Methods

| Method | Description |
| --- | --- |
| [apply(Task root, ITreeAlgorithm&lt;Task&gt; alg, int level)](#apply-com.aspose.tasks.Task-com.aspose.tasks.ITreeAlgorithm-com.aspose.tasks.Task--int-) | Applies specified algorithm to each task of a tree. |
| [filter(Task root, ICondition&lt;Task&gt; cond)](#filter-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | Builds new tree of tasks which satisfy the condition. |
| [find(Task root, ICondition&lt;Task&gt; cond)](#find-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | Finds a task which satisfy the condition in a tree of tasks. |
| [taskChildrenCount(Task task)](#taskChildrenCount-com.aspose.tasks.Task-) | Recursively calculates a number of task's children tasks through all levels. |
### TaskUtils() {#TaskUtils--}
```
public TaskUtils()
```


### apply(Task root, ITreeAlgorithm&lt;Task&gt; alg, int level) {#apply-com.aspose.tasks.Task-com.aspose.tasks.ITreeAlgorithm-com.aspose.tasks.Task--int-}
```
public static void apply(Task root, ITreeAlgorithm<Task> alg, int level)
```


Applies specified algorithm to each task of a tree.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | Root of the tree |
| alg | com.aspose.tasks.ITreeAlgorithm&lt;com.aspose.tasks.Task&gt; | Applied algorithm. |
| level | int | Level of the root task. |

### filter(Task root, ICondition&lt;Task&gt; cond) {#filter-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public static Task filter(Task root, ICondition<Task> cond)
```


Builds new tree of tasks which satisfy the condition.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | Root of the tree. |
| cond | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | Applied condition. |

**Returns:**
[Task](../../com.aspose.tasks/task) - Root of a new tree.
### find(Task root, ICondition&lt;Task&gt; cond) {#find-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public static Task find(Task root, ICondition<Task> cond)
```


Finds a task which satisfy the condition in a tree of tasks.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | Root of the tree. |
| cond | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | Applied condition. |

**Returns:**
[Task](../../com.aspose.tasks/task) - Task if task was found, otherwise null.
### taskChildrenCount(Task task) {#taskChildrenCount-com.aspose.tasks.Task-}
```
public static int taskChildrenCount(Task task)
```


Recursively calculates a number of task's children tasks through all levels.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | The task which children calculate. |

**Returns:**
int - The number of children.
