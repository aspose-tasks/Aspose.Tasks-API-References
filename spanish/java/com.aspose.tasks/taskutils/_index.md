---
title: "TaskUtils"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Clase auxiliar que proporciona operaciones útiles con tareas."
type: docs
weight: 307
url: /es/java/com.aspose.tasks/taskutils/
---

**Inheritance:**
java.lang.Object
```
public class TaskUtils
```

Clase auxiliar que proporciona operaciones útiles con tareas.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [TaskUtils()](#TaskUtils--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [apply(Task root, ITreeAlgorithm&lt;Task&gt; alg, int level)](#apply-com.aspose.tasks.Task-com.aspose.tasks.ITreeAlgorithm-com.aspose.tasks.Task--int-) | Aplica el algoritmo especificado a cada tarea de un árbol. |
| [filter(Task root, ICondition&lt;Task&gt; cond)](#filter-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | Construye un nuevo árbol de tareas que cumplen la condición. |
| [find(Task root, ICondition&lt;Task&gt; cond)](#find-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | Encuentra una tarea que satisface la condición en un árbol de tareas. |
| [taskChildrenCount(Task task)](#taskChildrenCount-com.aspose.tasks.Task-) | Calcula recursivamente el número de tareas hijas de una tarea a través de todos los niveles. |
### TaskUtils() {#TaskUtils--}
```
public TaskUtils()
```


### apply(Task root, ITreeAlgorithm&lt;Task&gt; alg, int level) {#apply-com.aspose.tasks.Task-com.aspose.tasks.ITreeAlgorithm-com.aspose.tasks.Task--int-}
```
public static void apply(Task root, ITreeAlgorithm<Task> alg, int level)
```


Aplica el algoritmo especificado a cada tarea de un árbol.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | Raíz del árbol |
| alg | com.aspose.tasks.ITreeAlgorithm&lt;com.aspose.tasks.Task&gt; | Algoritmo aplicado. |
| level | int | Nivel de la tarea raíz. |

### filter(Task root, ICondition&lt;Task&gt; cond) {#filter-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public static Task filter(Task root, ICondition<Task> cond)
```


Construye un nuevo árbol de tareas que cumplen la condición.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | Raíz del árbol. |
| cond | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | Condición aplicada. |

**Returns:**
[Task](../../com.aspose.tasks/task) - Root of a new tree.
### find(Task root, ICondition&lt;Task&gt; cond) {#find-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public static Task find(Task root, ICondition<Task> cond)
```


Encuentra una tarea que satisface la condición en un árbol de tareas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | Raíz del árbol. |
| cond | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | Condición aplicada. |

**Returns:**
[Task](../../com.aspose.tasks/task) - Task if task was found, otherwise null.
### taskChildrenCount(Task task) {#taskChildrenCount-com.aspose.tasks.Task-}
```
public static int taskChildrenCount(Task task)
```


Calcula recursivamente el número de tareas hijas de una tarea a través de todos los niveles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | La tarea que calculan los hijos. |

**Returns:**
int - El número de hijos.
