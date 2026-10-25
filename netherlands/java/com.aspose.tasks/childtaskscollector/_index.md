---
title: "ChildTasksCollector"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Verzamelt alle onderliggende taken."
type: docs
weight: 49
url: /nl/java/com.aspose.tasks/childtaskscollector/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.TreeAlgorithmBase
```
public class ChildTasksCollector extends TreeAlgorithmBase<Task>
```

Verzamelt alle onderliggende taken.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [ChildTasksCollector()](#ChildTasksCollector--) | Initialiseert een nieuw exemplaar van de [ChildTasksCollector](../../com.aspose.tasks/childtaskscollector) klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [alg(Task el, int level)](#alg-com.aspose.tasks.Task-int-) | Verwerkt het opgegeven object. |
| [getTasks()](#getTasks--) | Haalt een lijst op van verzamelde onderliggende objecten (taken). |
### ChildTasksCollector() {#ChildTasksCollector--}
```
public ChildTasksCollector()
```


Initialiseert een nieuw exemplaar van de [ChildTasksCollector](../../com.aspose.tasks/childtaskscollector) klasse.

### alg(Task el, int level) {#alg-com.aspose.tasks.Task-int-}
```
public void alg(Task el, int level)
```


Verwerkt het opgegeven object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | Object om te verwerken. |
| niveau | int | Boomknooppuntniveau. |

### getTasks() {#getTasks--}
```
public final List<Task> getTasks()
```


Haalt een lijst op van verzamelde onderliggende objecten (taken).

**Returns:**
java.util.List&lt;com.aspose.tasks.Task&gt; - een lijst van verzamelde onderliggende objecten (taken).
