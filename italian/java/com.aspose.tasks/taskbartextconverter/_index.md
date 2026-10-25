---
title: "TaskBarTextConverter"
second_title: "Aspose.Tasks for Java API Reference"
description: "Convertitore personalizzato dei dati delle attività in testo della barra."
type: docs
weight: 290
url: /it/java/com.aspose.tasks/taskbartextconverter/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.Delegate, com.aspose.ms.System.MulticastDelegate
```
public abstract class TaskBarTextConverter extends System.MulticastDelegate
```

Convertitore personalizzato dei dati dell'attività in testo della barra.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [TaskBarTextConverter()](#TaskBarTextConverter--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [invoke(Task task)](#invoke-com.aspose.tasks.Task-) | Convertitore personalizzato dei dati dell'attività in testo della barra. |
### TaskBarTextConverter() {#TaskBarTextConverter--}
```
public TaskBarTextConverter()
```


### invoke(Task task) {#invoke-com.aspose.tasks.Task-}
```
public abstract String invoke(Task task)
```


Convertitore personalizzato dei dati dell'attività in testo della barra.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Attività per la quale verrà renderizzato il testo della barra dell'attività. |

**Returns:**
java.lang.String - Testo da renderizzare per una barra corrispondente all'attività specificata.
