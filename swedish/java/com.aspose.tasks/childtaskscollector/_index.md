---
title: "ChildTasksCollector"
second_title: "Aspose.Tasks for Java API-referens"
description: "Samlar alla underuppgifter."
type: docs
weight: 49
url: /sv/java/com.aspose.tasks/childtaskscollector/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.TreeAlgorithmBase
```
public class ChildTasksCollector extends TreeAlgorithmBase<Task>
```

Samlar alla underuppgifter.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [ChildTasksCollector()](#ChildTasksCollector--) | Initierar en ny instans av klassen [ChildTasksCollector](../../com.aspose.tasks/childtaskscollector). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [alg(Task el, int level)](#alg-com.aspose.tasks.Task-int-) | Bearbetar det angivna objektet. |
| [getTasks()](#getTasks--) | Hämtar en lista med insamlade barnobjekt (uppgifter). |
### ChildTasksCollector() {#ChildTasksCollector--}
```
public ChildTasksCollector()
```


Initierar en ny instans av klassen [ChildTasksCollector](../../com.aspose.tasks/childtaskscollector).

### alg(Task el, int level) {#alg-com.aspose.tasks.Task-int-}
```
public void alg(Task el, int level)
```


Bearbetar det angivna objektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | Objekt att bearbeta. |
| nivå | int | Trädnodnivå. |

### getTasks() {#getTasks--}
```
public final List<Task> getTasks()
```


Hämtar en lista med insamlade barnobjekt (uppgifter).

**Returns:**
java.util.List&lt;com.aspose.tasks.Task&gt; - en lista med insamlade barnobjekt (uppgifter).
