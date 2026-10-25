---
title: "TreeAlgorithmBase"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Una clase base para implementaciones de ITreeAlgorithmltTgt"
type: docs
weight: 327
url: /es/java/com.aspose.tasks/treealgorithmbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ITreeAlgorithm
```
public abstract class TreeAlgorithmBase<T> implements ITreeAlgorithm<T>
```

Una clase base para implementaciones de ITreeAlgorithm&lt;T&gt;

T : El tipo de los elementos.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [TreeAlgorithmBase()](#TreeAlgorithmBase--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [alg(T el, int level)](#alg-T-int-) | Procesa un nodo de un árbol. |
| [postAlg(T el, int level)](#postAlg-T-int-) | Se llama después del procesamiento de un nodo de un árbol. |
| [preAlg(T el, int level)](#preAlg-T-int-) | Se llama antes del procesamiento de un nodo de un árbol. |
### TreeAlgorithmBase() {#TreeAlgorithmBase--}
```
public TreeAlgorithmBase()
```


### alg(T el, int level) {#alg-T-int-}
```
public abstract void alg(T el, int level)
```


Procesa un nodo de un árbol.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| el | T | Nodo a procesar. |
| level | int | Nivel del nodo del árbol. |

### postAlg(T el, int level) {#postAlg-T-int-}
```
public void postAlg(T el, int level)
```


Se llama después del procesamiento de un nodo de un árbol.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| el | T | Nodo a procesar. |
| level | int | Nivel del nodo del árbol. |

### preAlg(T el, int level) {#preAlg-T-int-}
```
public void preAlg(T el, int level)
```


Se llama antes del procesamiento de un nodo de un árbol.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| el | T | Nodo a procesar. |
| level | int | Nivel del nodo del árbol. |

