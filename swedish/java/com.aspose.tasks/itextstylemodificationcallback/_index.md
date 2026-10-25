---
title: "ITextStyleModificationCallback"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar en återuppringning som anropas innan TextStyle tillämpas på en tabellcell."
type: docs
weight: 383
url: /sv/java/com.aspose.tasks/itextstylemodificationcallback/
---
```
public interface ITextStyleModificationCallback
```

Representerar en återuppringning som anropas innan TextStyle tillämpas på en tabellcell.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [beforeTaskTextStyleApplied(TaskTextStyleEventArgs args)](#beforeTaskTextStyleApplied-com.aspose.tasks.TaskTextStyleEventArgs-) | Metoden som ska anropas innan rendering av en tabellcell för en uppgift rad i följande vyer: 'Gantt Chart', 'Task Sheet', 'Task Usage'. |
### beforeTaskTextStyleApplied(TaskTextStyleEventArgs args) {#beforeTaskTextStyleApplied-com.aspose.tasks.TaskTextStyleEventArgs-}
```
public abstract void beforeTaskTextStyleApplied(TaskTextStyleEventArgs args)
```


Metoden som ska anropas innan rendering av en tabellcell för en uppgift rad i följande vyer: 'Gantt Chart', 'Task Sheet', 'Task Usage'.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| args | [TaskTextStyleEventArgs](../../com.aspose.tasks/tasktextstyleeventargs) | Objektet [TaskTextStyleEventArgs](../../com.aspose.tasks/tasktextstyleeventargs). |

