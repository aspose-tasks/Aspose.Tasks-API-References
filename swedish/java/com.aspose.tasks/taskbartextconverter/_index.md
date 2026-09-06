---
title: "TaskBarTextConverter"
second_title: "Aspose.Tasks for Java API-referens"
description: "Anpassad konverterare av uppgiftsdata till stapeltext."
type: docs
weight: 290
url: /sv/java/com.aspose.tasks/taskbartextconverter/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.Delegate, com.aspose.ms.System.MulticastDelegate
```
public abstract class TaskBarTextConverter extends System.MulticastDelegate
```

Anpassad konverterare av uppgiftsdata till stapeltext.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [TaskBarTextConverter()](#TaskBarTextConverter--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [invoke(Task task)](#invoke-com.aspose.tasks.Task-) | Anpassad konverterare av uppgiftsdata till stapeltext. |
### TaskBarTextConverter() {#TaskBarTextConverter--}
```
public TaskBarTextConverter()
```


### invoke(Task task) {#invoke-com.aspose.tasks.Task-}
```
public abstract String invoke(Task task)
```


Anpassad konverterare av uppgiftsdata till stapeltext.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Uppgift för vilken stapelns text ska renderas. |

**Returns:**
java.lang.String - Text att rendera för en stapel som motsvarar den angivna uppgiften.
