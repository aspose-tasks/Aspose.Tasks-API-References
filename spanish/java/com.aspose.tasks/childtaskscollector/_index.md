---
title: "ChildTasksCollector"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Recopila todas las tareas secundarias."
type: docs
weight: 49
url: /es/java/com.aspose.tasks/childtaskscollector/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.TreeAlgorithmBase
```
public class ChildTasksCollector extends TreeAlgorithmBase<Task>
```

Recopila todas las tareas secundarias.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [ChildTasksCollector()](#ChildTasksCollector--) | Inicializa una nueva instancia de la clase [ChildTasksCollector](../../com.aspose.tasks/childtaskscollector). |
## Métodos

| Método | Descripción |
| --- | --- |
| [alg(Task el, int level)](#alg-com.aspose.tasks.Task-int-) | Procesa el objeto especificado. |
| [getTasks()](#getTasks--) | Obtiene una lista de objetos secundarios recopilados (tareas). |
### ChildTasksCollector() {#ChildTasksCollector--}
```
public ChildTasksCollector()
```


Inicializa una nueva instancia de la clase [ChildTasksCollector](../../com.aspose.tasks/childtaskscollector).

### alg(Task el, int level) {#alg-com.aspose.tasks.Task-int-}
```
public void alg(Task el, int level)
```


Procesa el objeto especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | Objeto a procesar. |
| level | int | Nivel del nodo del árbol. |

### getTasks() {#getTasks--}
```
public final List<Task> getTasks()
```


Obtiene una lista de objetos secundarios recopilados (tareas).

**Returns:**
java.util.List&lt;com.aspose.tasks.Task&gt; - una lista de objetos secundarios recopilados (tareas).
