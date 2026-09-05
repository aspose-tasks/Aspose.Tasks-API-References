---
title: "TaskBarTextConverter"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Aangepaste converter van takengegevens naar balktekst."
type: docs
weight: 290
url: /nl/java/com.aspose.tasks/taskbartextconverter/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.Delegate, com.aspose.ms.System.MulticastDelegate
```
public abstract class TaskBarTextConverter extends System.MulticastDelegate
```

Aangepaste converter van taakgegevens naar balktekst.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [TaskBarTextConverter()](#TaskBarTextConverter--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [invoke(Task task)](#invoke-com.aspose.tasks.Task-) | Aangepaste converter van taakgegevens naar balktekst. |
### TaskBarTextConverter() {#TaskBarTextConverter--}
```
public TaskBarTextConverter()
```


### invoke(Task task) {#invoke-com.aspose.tasks.Task-}
```
public abstract String invoke(Task task)
```


Aangepaste converter van taakgegevens naar balktekst.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Taak waarvoor de tekst van de taakbalk wordt weergegeven. |

**Returns:**
java.lang.String - Tekst om weer te geven voor een balk die overeenkomt met de opgegeven taak.
