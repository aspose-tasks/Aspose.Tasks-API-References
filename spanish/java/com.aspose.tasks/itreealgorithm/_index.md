---
title: "ITreeAlgorithm"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa un algoritmo que puede aplicarse a un árbol de objetos T."
type: docs
weight: 384
url: /es/java/com.aspose.tasks/itreealgorithm/
---
```
public interface ITreeAlgorithm<T>
```

Representa un algoritmo que puede aplicarse a un árbol de objetos `T`.

T : El tipo de objeto al que aplicar la interfaz del método.
## Métodos

| Método | Descripción |
| --- | --- |
| [alg(T el, int level)](#alg-T-int-) | Procesa un nodo de un árbol. |
| [postAlg(T el, int level)](#postAlg-T-int-) | Se llama después del procesamiento de un nodo de un árbol. |
| [preAlg(T el, int level)](#preAlg-T-int-) | Se llama antes del procesamiento de un nodo de un árbol. |
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
public abstract void postAlg(T el, int level)
```


Se llama después del procesamiento de un nodo de un árbol.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| el | T | Nodo a procesar. |
| level | int | Nivel del nodo del árbol. |

### preAlg(T el, int level) {#preAlg-T-int-}
```
public abstract void preAlg(T el, int level)
```


Se llama antes del procesamiento de un nodo de un árbol.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| el | T | Nodo a procesar. |
| level | int | Nivel del nodo del árbol. |

