---
title: "TaskBarTextConverter"
second_title: "Aspose.Tasks for Java API Reference"
description: "Benutzerdefinierter Konverter von Aufgabendaten zu Balkentext."
type: docs
weight: 290
url: /de/java/com.aspose.tasks/taskbartextconverter/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.Delegate, com.aspose.ms.System.MulticastDelegate
```
public abstract class TaskBarTextConverter extends System.MulticastDelegate
```

Benutzerdefinierter Konverter von Aufgabendaten zu Balkentext.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [TaskBarTextConverter()](#TaskBarTextConverter--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [invoke(Task task)](#invoke-com.aspose.tasks.Task-) | Benutzerdefinierter Konverter von Aufgabendaten zu Balkentext. |
### TaskBarTextConverter() {#TaskBarTextConverter--}
```
public TaskBarTextConverter()
```


### invoke(Task task) {#invoke-com.aspose.tasks.Task-}
```
public abstract String invoke(Task task)
```


Benutzerdefinierter Konverter von Aufgabendaten zu Balkentext.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Aufgabe, für die der Text der Aufgabenleiste gerendert wird. |

**Returns:**
java.lang.String - Text, der für einen Balken gerendert wird, der der angegebenen Aufgabe entspricht.
