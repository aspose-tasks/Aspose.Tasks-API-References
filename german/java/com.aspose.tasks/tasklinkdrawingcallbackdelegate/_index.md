---
title: "TaskLinkDrawingCallbackDelegate"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt einen Rückruf dar, der aufgerufen wird, wenn ein Aufgabenlink in einer Gantt-Diagrammansicht gerendert wird."
type: docs
weight: 298
url: /de/java/com.aspose.tasks/tasklinkdrawingcallbackdelegate/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.Delegate, com.aspose.ms.System.MulticastDelegate
```
public abstract class TaskLinkDrawingCallbackDelegate extends System.MulticastDelegate
```

Stellt einen Rückruf dar, der aufgerufen wird, wenn ein Aufgabenlink in einer Gantt-Diagrammansicht gerendert wird.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [TaskLinkDrawingCallbackDelegate()](#TaskLinkDrawingCallbackDelegate--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [invoke(TaskLinkDrawingArgs args)](#invoke-com.aspose.tasks.TaskLinkDrawingArgs-) | Stellt eine Methoden‑Callback‑Funktion dar, um das Zeichnen von Aufgabenverknüpfungen zu behandeln. |
### TaskLinkDrawingCallbackDelegate() {#TaskLinkDrawingCallbackDelegate--}
```
public TaskLinkDrawingCallbackDelegate()
```


### invoke(TaskLinkDrawingArgs args) {#invoke-com.aspose.tasks.TaskLinkDrawingArgs-}
```
public abstract void invoke(TaskLinkDrawingArgs args)
```


Stellt eine Methoden‑Callback‑Funktion dar, um das Zeichnen von Aufgabenverknüpfungen zu behandeln.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| args | [TaskLinkDrawingArgs](../../com.aspose.tasks/tasklinkdrawingargs) | die Instanz der [TaskLinkDrawingArgs](../../com.aspose.tasks/tasklinkdrawingargs)-Klasse, die die Callback‑Daten enthält. |

