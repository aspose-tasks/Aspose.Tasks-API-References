---
title: "IAlgorithm"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta un algoritmo che può essere applicato a un elenco di oggetti T."
type: docs
weight: 375
url: /it/java/com.aspose.tasks/ialgorithm/
---
```
public interface IAlgorithm<T>
```

Rappresenta un algoritmo che può essere applicato a un elenco di oggetti `T`.

T : Il tipo di oggetto a cui applicare l'interfaccia del metodo.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [alg(T el, int index)](#alg-T-int-) | Elabora un oggetto nell'elenco. |
| [postAlg(T el, int index)](#postAlg-T-int-) | Chiamato dopo l'elaborazione di un oggetto. |
| [preAlg(T el, int index)](#preAlg-T-int-) | Chiamato prima dell'elaborazione di un oggetto. |
### alg(T el, int index) {#alg-T-int-}
```
public abstract void alg(T el, int index)
```


Elabora un oggetto nell'elenco. Chiamato dopo [preAlg(T, int)](../../com.aspose.tasks/ialgorithm\#preAlg-T--int-);

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| el | T | Oggetto elaborato. |
| index | int | Indice dell'oggetto. |

### postAlg(T el, int index) {#postAlg-T-int-}
```
public abstract void postAlg(T el, int index)
```


Chiamato dopo l'elaborazione di un oggetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| el | T | Oggetto elaborato. |
| index | int | Indice dell'oggetto. |

### preAlg(T el, int index) {#preAlg-T-int-}
```
public abstract void preAlg(T el, int index)
```


Chiamato prima dell'elaborazione di un oggetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| el | T | Oggetto elaborato. |
| index | int | Indice dell'oggetto. |

