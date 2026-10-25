---
title: "TaskLinkDrawingCallbackDelegate"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een callback voor die wordt aangeroepen wanneer een taaklink wordt gerenderd in een Gantt-diagramweergave."
type: docs
weight: 298
url: /nl/java/com.aspose.tasks/tasklinkdrawingcallbackdelegate/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.Delegate, com.aspose.ms.System.MulticastDelegate
```
public abstract class TaskLinkDrawingCallbackDelegate extends System.MulticastDelegate
```

Stelt een callback voor die wordt aangeroepen wanneer een taaklink wordt gerenderd in een Gantt-diagramweergave.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [TaskLinkDrawingCallbackDelegate()](#TaskLinkDrawingCallbackDelegate--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [invoke(TaskLinkDrawingArgs args)](#invoke-com.aspose.tasks.TaskLinkDrawingArgs-) | Stelt een methodecallback voor die de taakkoppelings-tekengebeurtenis afhandelt. |
### TaskLinkDrawingCallbackDelegate() {#TaskLinkDrawingCallbackDelegate--}
```
public TaskLinkDrawingCallbackDelegate()
```


### invoke(TaskLinkDrawingArgs args) {#invoke-com.aspose.tasks.TaskLinkDrawingArgs-}
```
public abstract void invoke(TaskLinkDrawingArgs args)
```


Stelt een methodecallback voor die de taakkoppelings-tekengebeurtenis afhandelt.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| args | [TaskLinkDrawingArgs](../../com.aspose.tasks/tasklinkdrawingargs) | het exemplaar van de [TaskLinkDrawingArgs](../../com.aspose.tasks/tasklinkdrawingargs) klasse dat de callback-gegevens bevat. |

