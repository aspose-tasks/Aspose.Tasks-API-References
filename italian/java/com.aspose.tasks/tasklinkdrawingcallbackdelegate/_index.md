---
title: "TaskLinkDrawingCallbackDelegate"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta un callback che viene chiamato quando un collegamento dell'attività è renderizzato in una vista diagramma di Gantt."
type: docs
weight: 298
url: /it/java/com.aspose.tasks/tasklinkdrawingcallbackdelegate/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.Delegate, com.aspose.ms.System.MulticastDelegate
```
public abstract class TaskLinkDrawingCallbackDelegate extends System.MulticastDelegate
```

Rappresenta un callback che viene chiamato quando un collegamento dell'attività è renderizzato in una vista diagramma di Gantt.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [TaskLinkDrawingCallbackDelegate()](#TaskLinkDrawingCallbackDelegate--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [invoke(TaskLinkDrawingArgs args)](#invoke-com.aspose.tasks.TaskLinkDrawingArgs-) | Rappresenta un callback di metodo per gestire l'evento di disegno del collegamento attività. |
### TaskLinkDrawingCallbackDelegate() {#TaskLinkDrawingCallbackDelegate--}
```
public TaskLinkDrawingCallbackDelegate()
```


### invoke(TaskLinkDrawingArgs args) {#invoke-com.aspose.tasks.TaskLinkDrawingArgs-}
```
public abstract void invoke(TaskLinkDrawingArgs args)
```


Rappresenta un callback di metodo per gestire l'evento di disegno del collegamento attività.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| args | [TaskLinkDrawingArgs](../../com.aspose.tasks/tasklinkdrawingargs) | l'istanza della classe [TaskLinkDrawingArgs](../../com.aspose.tasks/tasklinkdrawingargs) che contiene i dati del callback. |

