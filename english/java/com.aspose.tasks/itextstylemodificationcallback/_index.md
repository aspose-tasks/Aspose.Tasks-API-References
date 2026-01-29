---
title: ITextStyleModificationCallback
second_title: Aspose.Tasks for Java API Reference
description: Represents a callback that is called before TextStyle is applied to a table cell.
type: docs
weight: 382
url: /java/com.aspose.tasks/itextstylemodificationcallback/
---
```
public interface ITextStyleModificationCallback
```

Represents a callback that is called before TextStyle is applied to a table cell.
## Methods

| Method | Description |
| --- | --- |
| [beforeTaskTextStyleApplied(TaskTextStyleEventArgs args)](#beforeTaskTextStyleApplied-com.aspose.tasks.TaskTextStyleEventArgs-) | The method to be called before rendering of a table cell for a task row in the following views: 'Gantt Chart', 'Task Sheet', 'Task Usage'. |
### beforeTaskTextStyleApplied(TaskTextStyleEventArgs args) {#beforeTaskTextStyleApplied-com.aspose.tasks.TaskTextStyleEventArgs-}
```
public abstract void beforeTaskTextStyleApplied(TaskTextStyleEventArgs args)
```


The method to be called before rendering of a table cell for a task row in the following views: 'Gantt Chart', 'Task Sheet', 'Task Usage'.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| args | [TaskTextStyleEventArgs](../../com.aspose.tasks/tasktextstyleeventargs) | The [TaskTextStyleEventArgs](../../com.aspose.tasks/tasktextstyleeventargs) object. |

