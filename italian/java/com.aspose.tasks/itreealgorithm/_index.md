---
title: "ITreeAlgorithm"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta un algoritmo che può essere applicato a un albero di oggetti T."
type: docs
weight: 384
url: /it/java/com.aspose.tasks/itreealgorithm/
---
```
public interface ITreeAlgorithm<T>
```

Rappresenta un algoritmo che può essere applicato a un albero di oggetti `T`.

T : Il tipo di oggetto a cui applicare l'interfaccia del metodo.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [alg(T el, int level)](#alg-T-int-) | Elabora un nodo di un albero. |
| [postAlg(T el, int level)](#postAlg-T-int-) | Chiamato dopo l'elaborazione di un nodo di un albero. |
| [preAlg(T el, int level)](#preAlg-T-int-) | Chiamato prima dell'elaborazione di un nodo di un albero. |
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
public abstract void postAlg(T el, int level)
```


Chiamato dopo l'elaborazione di un nodo di un albero.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| el | T | Nodo da elaborare. |
| level | int | Livello del nodo dell'albero. |

### preAlg(T el, int level) {#preAlg-T-int-}
```
public abstract void preAlg(T el, int level)
```


Chiamato prima dell'elaborazione di un nodo di un albero.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| el | T | Nodo da elaborare. |
| level | int | Livello del nodo dell'albero. |

