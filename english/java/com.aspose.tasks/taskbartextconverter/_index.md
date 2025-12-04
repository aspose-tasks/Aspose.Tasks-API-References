---
title: TaskBarTextConverter
second_title: Aspose.Tasks for Java API Reference
description: Custom converter of tasks data to bar text.
type: docs
weight: 289
url: /java/com.aspose.tasks/taskbartextconverter/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.Delegate, com.aspose.ms.System.MulticastDelegate
```
public abstract class TaskBarTextConverter extends System.MulticastDelegate
```

Custom converter of task's data to bar text.
## Constructors

| Constructor | Description |
| --- | --- |
| [TaskBarTextConverter()](#TaskBarTextConverter--) |  |
## Methods

| Method | Description |
| --- | --- |
| [invoke(Task task)](#invoke-com.aspose.tasks.Task-) | Custom converter of task's data to bar text. |
### TaskBarTextConverter() {#TaskBarTextConverter--}
```
public TaskBarTextConverter()
```


### invoke(Task task) {#invoke-com.aspose.tasks.Task-}
```
public abstract String invoke(Task task)
```


Custom converter of task's data to bar text.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Task for which task bar's text will be rendered. |

**Returns:**
java.lang.String - Text to render for a bar corresponding to the specified task.
