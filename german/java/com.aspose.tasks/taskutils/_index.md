---
title: "TaskUtils"
second_title: "Aspose.Tasks for Java API Reference"
description: "Hilfsklasse, die nützliche Operationen mit Aufgaben bereitstellt."
type: docs
weight: 307
url: /de/java/com.aspose.tasks/taskutils/
---

**Inheritance:**
java.lang.Object
```
public class TaskUtils
```

Hilfsklasse, die nützliche Operationen mit Aufgaben bereitstellt.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [TaskUtils()](#TaskUtils--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [apply(Task root, ITreeAlgorithm&lt;Task&gt; alg, int level)](#apply-com.aspose.tasks.Task-com.aspose.tasks.ITreeAlgorithm-com.aspose.tasks.Task--int-) | Wendet den angegebenen Algorithmus auf jede Aufgabe eines Baums an. |
| [filter(Task root, ICondition&lt;Task&gt; cond)](#filter-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | Erstellt einen neuen Aufgabenbaum, der die Bedingung erfüllt. |
| [find(Task root, ICondition&lt;Task&gt; cond)](#find-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | Findet eine Aufgabe, die die Bedingung in einem Aufgabenbaum erfüllt. |
| [taskChildrenCount(Task task)](#taskChildrenCount-com.aspose.tasks.Task-) | Berechnet rekursiv die Anzahl der Unteraufgaben einer Aufgabe über alle Ebenen hinweg. |
### TaskUtils() {#TaskUtils--}
```
public TaskUtils()
```


### apply(Task root, ITreeAlgorithm&lt;Task&gt; alg, int level) {#apply-com.aspose.tasks.Task-com.aspose.tasks.ITreeAlgorithm-com.aspose.tasks.Task--int-}
```
public static void apply(Task root, ITreeAlgorithm<Task> alg, int level)
```


Wendet den angegebenen Algorithmus auf jede Aufgabe eines Baums an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | Wurzel des Baums |
| alg | com.aspose.tasks.ITreeAlgorithm&lt;com.aspose.tasks.Task&gt; | Angewendeter Algorithmus. |
| Ebene | int | Ebene der Wurzelaufgabe. |

### filter(Task root, ICondition&lt;Task&gt; cond) {#filter-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public static Task filter(Task root, ICondition<Task> cond)
```


Erstellt einen neuen Aufgabenbaum, der die Bedingung erfüllt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | Wurzel des Baums. |
| cond | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | Angewendete Bedingung. |

**Returns:**
[Task](../../com.aspose.tasks/task) - Root of a new tree.
### find(Task root, ICondition&lt;Task&gt; cond) {#find-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public static Task find(Task root, ICondition<Task> cond)
```


Findet eine Aufgabe, die die Bedingung in einem Aufgabenbaum erfüllt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | Wurzel des Baums. |
| cond | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | Angewendete Bedingung. |

**Returns:**
[Task](../../com.aspose.tasks/task) - Task if task was found, otherwise null.
### taskChildrenCount(Task task) {#taskChildrenCount-com.aspose.tasks.Task-}
```
public static int taskChildrenCount(Task task)
```


Berechnet rekursiv die Anzahl der Unteraufgaben einer Aufgabe über alle Ebenen hinweg.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Die Aufgabe, deren Kinder berechnet werden. |

**Returns:**
int - Die Anzahl der Kinder.
