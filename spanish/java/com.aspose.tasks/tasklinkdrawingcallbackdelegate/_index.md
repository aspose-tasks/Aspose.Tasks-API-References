---
title: "TaskLinkDrawingCallbackDelegate"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa una devolución de llamada que se ejecuta cuando se renderiza un enlace de tarea en una vista de diagrama de Gantt."
type: docs
weight: 298
url: /es/java/com.aspose.tasks/tasklinkdrawingcallbackdelegate/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.Delegate, com.aspose.ms.System.MulticastDelegate
```
public abstract class TaskLinkDrawingCallbackDelegate extends System.MulticastDelegate
```

Representa una devolución de llamada que se ejecuta cuando se renderiza un enlace de tarea en una vista de diagrama de Gantt.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [TaskLinkDrawingCallbackDelegate()](#TaskLinkDrawingCallbackDelegate--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [invoke(TaskLinkDrawingArgs args)](#invoke-com.aspose.tasks.TaskLinkDrawingArgs-) | Representa una devolución de llamada de método para manejar el evento de dibujo del enlace de tarea. |
### TaskLinkDrawingCallbackDelegate() {#TaskLinkDrawingCallbackDelegate--}
```
public TaskLinkDrawingCallbackDelegate()
```


### invoke(TaskLinkDrawingArgs args) {#invoke-com.aspose.tasks.TaskLinkDrawingArgs-}
```
public abstract void invoke(TaskLinkDrawingArgs args)
```


Representa una devolución de llamada de método para manejar el evento de dibujo del enlace de tarea.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| args | [TaskLinkDrawingArgs](../../com.aspose.tasks/tasklinkdrawingargs) | la instancia de la clase [TaskLinkDrawingArgs](../../com.aspose.tasks/tasklinkdrawingargs) que contiene los datos de la devolución de llamada. |

