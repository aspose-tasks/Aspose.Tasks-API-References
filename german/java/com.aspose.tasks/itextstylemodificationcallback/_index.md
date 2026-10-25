---
title: "ITextStyleModificationCallback"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt einen Callback dar, der aufgerufen wird, bevor TextStyle auf eine Tabellenzelle angewendet wird."
type: docs
weight: 383
url: /de/java/com.aspose.tasks/itextstylemodificationcallback/
---
```
public interface ITextStyleModificationCallback
```

Stellt einen Callback dar, der aufgerufen wird, bevor TextStyle auf eine Tabellenzelle angewendet wird.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [beforeTaskTextStyleApplied(TaskTextStyleEventArgs args)](#beforeTaskTextStyleApplied-com.aspose.tasks.TaskTextStyleEventArgs-) | Die Methode, die vor dem Rendern einer Tabellenzelle für eine Aufgabenzeile in den folgenden Ansichten aufgerufen wird: 'Gantt Chart', 'Task Sheet', 'Task Usage'. |
### beforeTaskTextStyleApplied(TaskTextStyleEventArgs args) {#beforeTaskTextStyleApplied-com.aspose.tasks.TaskTextStyleEventArgs-}
```
public abstract void beforeTaskTextStyleApplied(TaskTextStyleEventArgs args)
```


Die Methode, die vor dem Rendern einer Tabellenzelle für eine Aufgabenzeile in den folgenden Ansichten aufgerufen wird: 'Gantt Chart', 'Task Sheet', 'Task Usage'.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| args | [TaskTextStyleEventArgs](../../com.aspose.tasks/tasktextstyleeventargs) | Das [TaskTextStyleEventArgs](../../com.aspose.tasks/tasktextstyleeventargs)-Objekt. |

