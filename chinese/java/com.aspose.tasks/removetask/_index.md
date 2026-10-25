---
title: "RemoveTask"
second_title: "Aspose.Tasks for Java API 参考"
description: "从任务树中删除指定的任务。"
type: docs
weight: 246
url: /zh/java/com.aspose.tasks/removetask/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ITreeAlgorithm
```
public class RemoveTask implements ITreeAlgorithm<Task>
```

从任务树中删除指定的任务。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [RemoveTask(Task task)](#RemoveTask-com.aspose.tasks.Task-) | 初始化一个新的 [RemoveTask](../../com.aspose.tasks/removetask) 类的实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [alg(Task el, int level)](#alg-com.aspose.tasks.Task-int-) | 什么也不做。 |
| [postAlg(Task el, int level)](#postAlg-com.aspose.tasks.Task-int-) | 什么也不做。 |
| [preAlg(Task el, int level)](#preAlg-com.aspose.tasks.Task-int-) | 从指定的父任务中移除该任务。 |
### RemoveTask(Task task) {#RemoveTask-com.aspose.tasks.Task-}
```
public RemoveTask(Task task)
```


初始化一个新的 [RemoveTask](../../com.aspose.tasks/removetask) 类的实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | 要移除的任务。 |

### alg(Task el, int level) {#alg-com.aspose.tasks.Task-int-}
```
public final void alg(Task el, int level)
```


什么也不做。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | 要处理的对象。 |
| 级别 | int | 树节点级别。 |

### postAlg(Task el, int level) {#postAlg-com.aspose.tasks.Task-int-}
```
public final void postAlg(Task el, int level)
```


什么也不做。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | 要处理的对象。 |
| 级别 | int | 树节点级别。 |

### preAlg(Task el, int level) {#preAlg-com.aspose.tasks.Task-int-}
```
public final void preAlg(Task el, int level)
```


从指定的父任务中移除该任务。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | 父任务。 |
| 级别 | int | 树节点级别。 |

