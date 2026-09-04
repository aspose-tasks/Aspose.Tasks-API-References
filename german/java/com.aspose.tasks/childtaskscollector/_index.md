---
title: "ChildTasksCollector"
second_title: "Aspose.Tasks for Java API Reference"
description: "Sammelt alle untergeordneten Aufgaben."
type: docs
weight: 49
url: /de/java/com.aspose.tasks/childtaskscollector/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.TreeAlgorithmBase
```
public class ChildTasksCollector extends TreeAlgorithmBase<Task>
```

Sammelt alle untergeordneten Aufgaben.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ChildTasksCollector()](#ChildTasksCollector--) | Initialisiert eine neue Instanz der Klasse [ChildTasksCollector](../../com.aspose.tasks/childtaskscollector). |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [alg(Task el, int level)](#alg-com.aspose.tasks.Task-int-) | Verarbeitet das angegebene Objekt. |
| [getTasks()](#getTasks--) | Gibt eine Liste gesammelter Kindobjekte (Aufgaben) zurück. |
### ChildTasksCollector() {#ChildTasksCollector--}
```
public ChildTasksCollector()
```


Initialisiert eine neue Instanz der Klasse [ChildTasksCollector](../../com.aspose.tasks/childtaskscollector).

### alg(Task el, int level) {#alg-com.aspose.tasks.Task-int-}
```
public void alg(Task el, int level)
```


Verarbeitet das angegebene Objekt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | Zu verarbeitendes Objekt. |
| Ebene | int | Baumknotenebene. |

### getTasks() {#getTasks--}
```
public final List<Task> getTasks()
```


Gibt eine Liste gesammelter Kindobjekte (Aufgaben) zurück.

**Returns:**
java.util.List&lt;com.aspose.tasks.Task&gt; - eine Liste gesammelter Kindobjekte (Aufgaben).
