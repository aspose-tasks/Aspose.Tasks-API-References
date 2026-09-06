---
title: "IAlgorithm"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar en algoritm som kan tillämpas på en lista med objekt T."
type: docs
weight: 375
url: /sv/java/com.aspose.tasks/ialgorithm/
---
```
public interface IAlgorithm<T>
```

Representerar en algoritm som kan tillämpas på en lista av objekt `T`.

T : Typen av objekt som metodgränssnittet ska tillämpas på.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [alg(T el, int index)](#alg-T-int-) | Bearbetar ett objekt i listan. |
| [postAlg(T el, int index)](#postAlg-T-int-) | Kallas efter bearbetning av ett objekt. |
| [preAlg(T el, int index)](#preAlg-T-int-) | Kallas före bearbetning av ett objekt. |
### alg(T el, int index) {#alg-T-int-}
```
public abstract void alg(T el, int index)
```


Bearbetar ett objekt i listan. Kallas efter [preAlg(T, int)](../../com.aspose.tasks/ialgorithm\#preAlg-T--int-);

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| el | T | Bearbetat objekt. |
| index | int | Index för objektet. |

### postAlg(T el, int index) {#postAlg-T-int-}
```
public abstract void postAlg(T el, int index)
```


Kallas efter bearbetning av ett objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| el | T | Bearbetat objekt. |
| index | int | Index för objektet. |

### preAlg(T el, int index) {#preAlg-T-int-}
```
public abstract void preAlg(T el, int index)
```


Kallas före bearbetning av ett objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| el | T | Bearbetat objekt. |
| index | int | Index för objektet. |

