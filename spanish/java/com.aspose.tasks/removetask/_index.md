---
title: "RemoveTask"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Elimina la tarea especificada de un árbol de tareas."
type: docs
weight: 246
url: /es/java/com.aspose.tasks/removetask/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ITreeAlgorithm
```
public class RemoveTask implements ITreeAlgorithm<Task>
```

Elimina la tarea especificada de un árbol de tareas.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [RemoveTask(Task task)](#RemoveTask-com.aspose.tasks.Task-) | Inicializa una nueva instancia de la clase [RemoveTask](../../com.aspose.tasks/removetask). |
## Métodos

| Método | Descripción |
| --- | --- |
| [alg(Task el, int level)](#alg-com.aspose.tasks.Task-int-) | No hacer nada. |
| [postAlg(Task el, int level)](#postAlg-com.aspose.tasks.Task-int-) | No hacer nada. |
| [preAlg(Task el, int level)](#preAlg-com.aspose.tasks.Task-int-) | Elimina la tarea del padre especificado. |
### RemoveTask(Task task) {#RemoveTask-com.aspose.tasks.Task-}
```
public RemoveTask(Task task)
```


Inicializa una nueva instancia de la clase [RemoveTask](../../com.aspose.tasks/removetask).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Tarea a eliminar. |

### alg(Task el, int level) {#alg-com.aspose.tasks.Task-int-}
```
public final void alg(Task el, int level)
```


No hacer nada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | Objeto a procesar. |
| level | int | Nivel del nodo del árbol. |

### postAlg(Task el, int level) {#postAlg-com.aspose.tasks.Task-int-}
```
public final void postAlg(Task el, int level)
```


No hacer nada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | Objeto a procesar. |
| level | int | Nivel del nodo del árbol. |

### preAlg(Task el, int level) {#preAlg-com.aspose.tasks.Task-int-}
```
public final void preAlg(Task el, int level)
```


Elimina la tarea del padre especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | Tarea padre. |
| level | int | Nivel del nodo del árbol. |

