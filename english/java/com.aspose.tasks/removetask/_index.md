---
title: RemoveTask
second_title: Aspose.Tasks for Java API Reference
description: Removes the specified task from a tree of tasks.
type: docs
weight: 245
url: /java/com.aspose.tasks/removetask/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ITreeAlgorithm
```
public class RemoveTask implements ITreeAlgorithm<Task>
```

Removes the specified task from a tree of tasks.
## Constructors

| Constructor | Description |
| --- | --- |
| [RemoveTask(Task task)](#RemoveTask-com.aspose.tasks.Task-) | Initializes a new instance of the [RemoveTask](../../com.aspose.tasks/removetask) class. |
## Methods

| Method | Description |
| --- | --- |
| [alg(Task el, int level)](#alg-com.aspose.tasks.Task-int-) | Do nothing. |
| [postAlg(Task el, int level)](#postAlg-com.aspose.tasks.Task-int-) | Do nothing. |
| [preAlg(Task el, int level)](#preAlg-com.aspose.tasks.Task-int-) | Removes the task from the specified parent task. |
### RemoveTask(Task task) {#RemoveTask-com.aspose.tasks.Task-}
```
public RemoveTask(Task task)
```


Initializes a new instance of the [RemoveTask](../../com.aspose.tasks/removetask) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Task to remove. |

### alg(Task el, int level) {#alg-com.aspose.tasks.Task-int-}
```
public final void alg(Task el, int level)
```


Do nothing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | Object to process. |
| level | int | Tree node level. |

### postAlg(Task el, int level) {#postAlg-com.aspose.tasks.Task-int-}
```
public final void postAlg(Task el, int level)
```


Do nothing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | Object to process. |
| level | int | Tree node level. |

### preAlg(Task el, int level) {#preAlg-com.aspose.tasks.Task-int-}
```
public final void preAlg(Task el, int level)
```


Removes the task from the specified parent task.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | Parent task. |
| level | int | Tree node level. |

