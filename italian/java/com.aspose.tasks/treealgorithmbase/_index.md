---
title: "TreeAlgorithmBase"
second_title: "Aspose.Tasks for Java API Reference"
description: "Una classe base per le implementazioni di ITreeAlgorithmltTgt"
type: docs
weight: 327
url: /it/java/com.aspose.tasks/treealgorithmbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ITreeAlgorithm
```
public abstract class TreeAlgorithmBase<T> implements ITreeAlgorithm<T>
```

Una classe base per le implementazioni di ITreeAlgorithm&lt;T&gt;

T : Il tipo degli elementi.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [TreeAlgorithmBase()](#TreeAlgorithmBase--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [alg(T el, int level)](#alg-T-int-) | Elabora un nodo di un albero. |
| [postAlg(T el, int level)](#postAlg-T-int-) | Chiamato dopo l'elaborazione di un nodo di un albero. |
| [preAlg(T el, int level)](#preAlg-T-int-) | Chiamato prima dell'elaborazione di un nodo di un albero. |
### TreeAlgorithmBase() {#TreeAlgorithmBase--}
```
public TreeAlgorithmBase()
```


### alg(T el, int level) {#alg-T-int-}
```
public abstract void alg(T el, int level)
```


Elabora un nodo di un albero.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| el | T | Nodo da elaborare. |
| level | int | Livello del nodo dell'albero. |

### postAlg(T el, int level) {#postAlg-T-int-}
```
public void postAlg(T el, int level)
```


Chiamato dopo l'elaborazione di un nodo di un albero.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| el | T | Nodo da elaborare. |
| level | int | Livello del nodo dell'albero. |

### preAlg(T el, int level) {#preAlg-T-int-}
```
public void preAlg(T el, int level)
```


Chiamato prima dell'elaborazione di un nodo di un albero.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| el | T | Nodo da elaborare. |
| level | int | Livello del nodo dell'albero. |

