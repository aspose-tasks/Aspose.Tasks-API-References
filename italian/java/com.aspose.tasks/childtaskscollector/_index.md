---
title: "ChildTasksCollector"
second_title: "Aspose.Tasks for Java API Reference"
description: "Raccoglie tutte le attività figlio."
type: docs
weight: 49
url: /it/java/com.aspose.tasks/childtaskscollector/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.TreeAlgorithmBase
```
public class ChildTasksCollector extends TreeAlgorithmBase<Task>
```

Raccoglie tutte le attività figlio.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [ChildTasksCollector()](#ChildTasksCollector--) | Inizializza una nuova istanza della classe [ChildTasksCollector](../../com.aspose.tasks/childtaskscollector). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [alg(Task el, int level)](#alg-com.aspose.tasks.Task-int-) | Elabora l'oggetto specificato. |
| [getTasks()](#getTasks--) | Restituisce un elenco di oggetti figlio raccolti (attività). |
### ChildTasksCollector() {#ChildTasksCollector--}
```
public ChildTasksCollector()
```


Inizializza una nuova istanza della classe [ChildTasksCollector](../../com.aspose.tasks/childtaskscollector).

### alg(Task el, int level) {#alg-com.aspose.tasks.Task-int-}
```
public void alg(Task el, int level)
```


Elabora l'oggetto specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | Oggetto da elaborare. |
| level | int | Livello del nodo dell'albero. |

### getTasks() {#getTasks--}
```
public final List<Task> getTasks()
```


Restituisce un elenco di oggetti figlio raccolti (attività).

**Returns:**
java.util.List&lt;com.aspose.tasks.Task&gt; - un elenco di oggetti figlio raccolti (attività).
