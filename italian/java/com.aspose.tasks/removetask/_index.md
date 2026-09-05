---
title: "RemoveTask"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rimuove l'attività specificata da un albero di attività."
type: docs
weight: 246
url: /it/java/com.aspose.tasks/removetask/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ITreeAlgorithm
```
public class RemoveTask implements ITreeAlgorithm<Task>
```

Rimuove l'attività specificata da un albero di attività.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [RemoveTask(Task task)](#RemoveTask-com.aspose.tasks.Task-) | Inizializza una nuova istanza della classe [RemoveTask](../../com.aspose/tasks/removetask). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [alg(Task el, int level)](#alg-com.aspose.tasks.Task-int-) | Non fare nulla. |
| [postAlg(Task el, int level)](#postAlg-com.aspose.tasks.Task-int-) | Non fare nulla. |
| [preAlg(Task el, int level)](#preAlg-com.aspose.tasks.Task-int-) | Rimuove l'attività dal task padre specificato. |
### RemoveTask(Task task) {#RemoveTask-com.aspose.tasks.Task-}
```
public RemoveTask(Task task)
```


Inizializza una nuova istanza della classe [RemoveTask](../../com.aspose/tasks/removetask).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Attività da rimuovere. |

### alg(Task el, int level) {#alg-com.aspose.tasks.Task-int-}
```
public final void alg(Task el, int level)
```


Non fare nulla.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | Oggetto da elaborare. |
| level | int | Livello del nodo dell'albero. |

### postAlg(Task el, int level) {#postAlg-com.aspose.tasks.Task-int-}
```
public final void postAlg(Task el, int level)
```


Non fare nulla.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | Oggetto da elaborare. |
| level | int | Livello del nodo dell'albero. |

### preAlg(Task el, int level) {#preAlg-com.aspose.tasks.Task-int-}
```
public final void preAlg(Task el, int level)
```


Rimuove l'attività dal task padre specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | Task padre. |
| level | int | Livello del nodo dell'albero. |

