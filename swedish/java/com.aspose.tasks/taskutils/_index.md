---
title: "TaskUtils"
second_title: "Aspose.Tasks for Java API-referens"
description: "Hjälparklass som tillhandahåller användbara operationer med uppgifter."
type: docs
weight: 307
url: /sv/java/com.aspose.tasks/taskutils/
---

**Inheritance:**
java.lang.Object
```
public class TaskUtils
```

Hjälparklass som tillhandahåller användbara operationer med uppgifter.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [TaskUtils()](#TaskUtils--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [apply(Task root, ITreeAlgorithm&lt;Task&gt; alg, int level)](#apply-com.aspose.tasks.Task-com.aspose.tasks.ITreeAlgorithm-com.aspose.tasks.Task--int-) | Tillämpar angiven algoritm på varje uppgift i ett träd. |
| [filter(Task root, ICondition&lt;Task&gt; cond)](#filter-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | Bygger ett nytt träd av uppgifter som uppfyller villkoret. |
| [find(Task root, ICondition&lt;Task&gt; cond)](#find-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | Hittar en uppgift som uppfyller villkoret i ett träd av uppgifter. |
| [taskChildrenCount(Task task)](#taskChildrenCount-com.aspose.tasks.Task-) | Beräknar rekursivt antalet underuppgifter för en uppgift genom alla nivåer. |
### TaskUtils() {#TaskUtils--}
```
public TaskUtils()
```


### apply(Task root, ITreeAlgorithm&lt;Task&gt; alg, int level) {#apply-com.aspose.tasks.Task-com.aspose.tasks.ITreeAlgorithm-com.aspose.tasks.Task--int-}
```
public static void apply(Task root, ITreeAlgorithm<Task> alg, int level)
```


Tillämpar angiven algoritm på varje uppgift i ett träd.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | Roten av trädet |
| alg | com.aspose.tasks.ITreeAlgorithm&lt;com.aspose.tasks.Task&gt; | Tillämpad algoritm. |
| nivå | int | Nivå för rotuppgiften. |

### filter(Task root, ICondition&lt;Task&gt; cond) {#filter-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public static Task filter(Task root, ICondition<Task> cond)
```


Bygger ett nytt träd av uppgifter som uppfyller villkoret.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | Roten av trädet. |
| cond | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | Tillämpat villkor. |

**Returns:**
[Task](../../com.aspose.tasks/task) - Root of a new tree.
### find(Task root, ICondition&lt;Task&gt; cond) {#find-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public static Task find(Task root, ICondition<Task> cond)
```


Hittar en uppgift som uppfyller villkoret i ett träd av uppgifter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | Roten av trädet. |
| cond | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | Tillämpat villkor. |

**Returns:**
[Task](../../com.aspose.tasks/task) - Task if task was found, otherwise null.
### taskChildrenCount(Task task) {#taskChildrenCount-com.aspose.tasks.Task-}
```
public static int taskChildrenCount(Task task)
```


Beräknar rekursivt antalet underuppgifter för en uppgift genom alla nivåer.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Uppgiften vars barn beräknas. |

**Returns:**
int - Antalet barn.
