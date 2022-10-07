---
title: ChildTasksCollector
second_title: Aspose.Tasks for Java API Reference
description: Collects all child tasks.
type: docs
weight: 49
url: /java/com.aspose.tasks/childtaskscollector/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.TreeAlgorithmBase
```
public class ChildTasksCollector extends TreeAlgorithmBase<Task>
```

Collects all child tasks.
## Constructors

| Constructor | Description |
| --- | --- |
| [ChildTasksCollector()](#ChildTasksCollector--) | Initializes a new instance of the [ChildTasksCollector](../../com.aspose.tasks/childtaskscollector) class. |
## Methods

| Method | Description |
| --- | --- |
| [alg(Task el, int level)](#alg-com.aspose.tasks.Task-int-) | Processes the specified object. |
| [getTasks()](#getTasks--) | Gets a list collected child objects (tasks). |
### ChildTasksCollector() {#ChildTasksCollector--}
```
public ChildTasksCollector()
```


Initializes a new instance of the [ChildTasksCollector](../../com.aspose.tasks/childtaskscollector) class.

### alg(Task el, int level) {#alg-com.aspose.tasks.Task-int-}
```
public void alg(Task el, int level)
```


Processes the specified object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | Object to process. |
| level | int | Tree node level. |

### getTasks() {#getTasks--}
```
public final List<Task> getTasks()
```


Gets a list collected child objects (tasks).

**Returns:**
java.util.List&lt;com.aspose.tasks.Task&gt; - a list collected child objects (tasks).
