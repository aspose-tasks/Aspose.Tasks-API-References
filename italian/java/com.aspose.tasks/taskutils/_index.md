---
title: "TaskUtils"
second_title: "Aspose.Tasks for Java API Reference"
description: "Classe di supporto che fornisce operazioni utili con le attività."
type: docs
weight: 307
url: /it/java/com.aspose.tasks/taskutils/
---

**Inheritance:**
java.lang.Object
```
public class TaskUtils
```

Classe di supporto che fornisce operazioni utili con le attività.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [TaskUtils()](#TaskUtils--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [apply(Task root, ITreeAlgorithm&lt;Task&gt; alg, int level)](#apply-com.aspose.tasks.Task-com.aspose.tasks.ITreeAlgorithm-com.aspose.tasks.Task--int-) | Applica l'algoritmo specificato a ciascuna attività di un albero. |
| [filter(Task root, ICondition&lt;Task&gt; cond)](#filter-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | Costruisce un nuovo albero di attività che soddisfano la condizione. |
| [find(Task root, ICondition&lt;Task&gt; cond)](#find-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | Trova un'attività che soddisfa la condizione in un albero di attività. |
| [taskChildrenCount(Task task)](#taskChildrenCount-com.aspose.tasks.Task-) | Calcola ricorsivamente il numero di attività figlie di un'attività attraverso tutti i livelli. |
### TaskUtils() {#TaskUtils--}
```
public TaskUtils()
```


### apply(Task root, ITreeAlgorithm&lt;Task&gt; alg, int level) {#apply-com.aspose.tasks.Task-com.aspose.tasks.ITreeAlgorithm-com.aspose.tasks.Task--int-}
```
public static void apply(Task root, ITreeAlgorithm<Task> alg, int level)
```


Applica l'algoritmo specificato a ciascuna attività di un albero.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | Radice dell'albero |
| alg | com.aspose.tasks.ITreeAlgorithm&lt;com.aspose.tasks.Task&gt; | Algoritmo applicato. |
| level | int | Livello dell'attività radice. |

### filter(Task root, ICondition&lt;Task&gt; cond) {#filter-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public static Task filter(Task root, ICondition<Task> cond)
```


Costruisce un nuovo albero di attività che soddisfano la condizione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | Radice dell'albero. |
| cond | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | Condizione applicata. |

**Returns:**
[Task](../../com.aspose.tasks/task) - Root of a new tree.
### find(Task root, ICondition&lt;Task&gt; cond) {#find-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public static Task find(Task root, ICondition<Task> cond)
```


Trova un'attività che soddisfa la condizione in un albero di attività.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | Radice dell'albero. |
| cond | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | Condizione applicata. |

**Returns:**
[Task](../../com.aspose.tasks/task) - Task if task was found, otherwise null.
### taskChildrenCount(Task task) {#taskChildrenCount-com.aspose.tasks.Task-}
```
public static int taskChildrenCount(Task task)
```


Calcola ricorsivamente il numero di attività figlie di un'attività attraverso tutti i livelli.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | L'attività di cui calcolare i figli. |

**Returns:**
int - Il numero di figli.
