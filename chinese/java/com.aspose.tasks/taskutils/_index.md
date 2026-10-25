---
title: "TaskUtils"
second_title: "Aspose.Tasks for Java API 参考"
description: "提供任务有用操作的帮助类。"
type: docs
weight: 307
url: /zh/java/com.aspose.tasks/taskutils/
---

**Inheritance:**
java.lang.Object
```
public class TaskUtils
```

提供任务有用操作的帮助类。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [TaskUtils()](#TaskUtils--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [apply(Task root, ITreeAlgorithm&lt;Task&gt; alg, int level)](#apply-com.aspose.tasks.Task-com.aspose.tasks.ITreeAlgorithm-com.aspose.tasks.Task--int-) | 将指定的算法应用于树中的每个任务。 |
| [filter(Task root, ICondition&lt;Task&gt; cond)](#filter-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | 构建满足条件的任务新树。 |
| [find(Task root, ICondition&lt;Task&gt; cond)](#find-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | 在任务树中查找满足条件的任务。 |
| [taskChildrenCount(Task task)](#taskChildrenCount-com.aspose.tasks.Task-) | 递归计算任务在所有层级中的子任务数量。 |
### TaskUtils() {#TaskUtils--}
```
public TaskUtils()
```


### apply(Task root, ITreeAlgorithm&lt;Task&gt; alg, int level) {#apply-com.aspose.tasks.Task-com.aspose.tasks.ITreeAlgorithm-com.aspose.tasks.Task--int-}
```
public static void apply(Task root, ITreeAlgorithm<Task> alg, int level)
```


将指定的算法应用于树中的每个任务。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | 树的根节点 |
| alg | com.aspose.tasks.ITreeAlgorithm&lt;com.aspose.tasks.Task&gt; | 已应用的算法。 |
| 级别 | int | 根任务的级别。 |

### filter(Task root, ICondition&lt;Task&gt; cond) {#filter-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public static Task filter(Task root, ICondition<Task> cond)
```


构建满足条件的任务新树。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | 树的根节点。 |
| cond | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | 已应用的条件。 |

**Returns:**
[Task](../../com.aspose.tasks/task) - Root of a new tree.
### find(Task root, ICondition&lt;Task&gt; cond) {#find-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public static Task find(Task root, ICondition<Task> cond)
```


在任务树中查找满足条件的任务。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | 树的根节点。 |
| cond | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | 已应用的条件。 |

**Returns:**
[Task](../../com.aspose.tasks/task) - Task if task was found, otherwise null.
### taskChildrenCount(Task task) {#taskChildrenCount-com.aspose.tasks.Task-}
```
public static int taskChildrenCount(Task task)
```


递归计算任务在所有层级中的子任务数量。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | 用于计算子任务的任务。 |

**Returns:**
int - 子项的数量。
