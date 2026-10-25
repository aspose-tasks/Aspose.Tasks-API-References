---
title: "IAlgorithm"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa un algoritmo que puede aplicarse a una lista de objetos T."
type: docs
weight: 375
url: /es/java/com.aspose.tasks/ialgorithm/
---
```
public interface IAlgorithm<T>
```

Representa un algoritmo que puede aplicarse a una lista de objetos `T`.

T : El tipo de objeto al que aplicar la interfaz del método.
## Métodos

| Método | Descripción |
| --- | --- |
| [alg(T el, int index)](#alg-T-int-) | Procesa un objeto en la lista. |
| [postAlg(T el, int index)](#postAlg-T-int-) | Se llama después del procesamiento de un objeto. |
| [preAlg(T el, int index)](#preAlg-T-int-) | Se llama antes del procesamiento de un objeto. |
### alg(T el, int index) {#alg-T-int-}
```
public abstract void alg(T el, int index)
```


Procesa un objeto en la lista. Llamado después de [preAlg(T, int)](../../com.aspose.tasks/ialgorithm\#preAlg-T--int-);

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| el | T | Objeto procesado. |
| índice | int | Índice del objeto. |

### postAlg(T el, int index) {#postAlg-T-int-}
```
public abstract void postAlg(T el, int index)
```


Se llama después del procesamiento de un objeto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| el | T | Objeto procesado. |
| índice | int | Índice del objeto. |

### preAlg(T el, int index) {#preAlg-T-int-}
```
public abstract void preAlg(T el, int index)
```


Se llama antes del procesamiento de un objeto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| el | T | Objeto procesado. |
| índice | int | Índice del objeto. |

