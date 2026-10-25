---
title: "ITextStyleModificationCallback"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een callback voor die wordt aangeroepen voordat TextStyle wordt toegepast op een tabelcel."
type: docs
weight: 383
url: /nl/java/com.aspose.tasks/itextstylemodificationcallback/
---
```
public interface ITextStyleModificationCallback
```

Stelt een callback voor die wordt aangeroepen voordat TextStyle wordt toegepast op een tabelcel.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [beforeTaskTextStyleApplied(TaskTextStyleEventArgs args)](#beforeTaskTextStyleApplied-com.aspose.tasks.TaskTextStyleEventArgs-) | De methode die moet worden aangeroepen vóór het renderen van een tabelcel voor een taakrij in de volgende weergaven: 'Gantt Chart', 'Task Sheet', 'Task Usage'. |
### beforeTaskTextStyleApplied(TaskTextStyleEventArgs args) {#beforeTaskTextStyleApplied-com.aspose.tasks.TaskTextStyleEventArgs-}
```
public abstract void beforeTaskTextStyleApplied(TaskTextStyleEventArgs args)
```


De methode die moet worden aangeroepen vóór het renderen van een tabelcel voor een taakrij in de volgende weergaven: 'Gantt Chart', 'Task Sheet', 'Task Usage'.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| args | [TaskTextStyleEventArgs](../../com.aspose.tasks/tasktextstyleeventargs) | Het [TaskTextStyleEventArgs](../../com.aspose.tasks/tasktextstyleeventargs) object. |

