---
title: "ITreeAlgorithm"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar en algoritm som kan tillämpas på ett träd av objekt T."
type: docs
weight: 384
url: /sv/java/com.aspose.tasks/itreealgorithm/
---
```
public interface ITreeAlgorithm<T>
```

Representerar en algoritm som kan tillämpas på ett träd av objekt `T`.

T : Typen av objekt som metodgränssnittet ska tillämpas på.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [alg(T el, int level)](#alg-T-int-) | Bearbetar en nod i ett träd. |
| [postAlg(T el, int level)](#postAlg-T-int-) | Kallas efter bearbetning av en nod i ett träd. |
| [preAlg(T el, int level)](#preAlg-T-int-) | Kallas före bearbetning av en nod i ett träd. |
### alg(T el, int level) {#alg-T-int-}
```
public abstract void alg(T el, int level)
```


Bearbetar en nod i ett träd.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| el | T | Nod att bearbeta. |
| nivå | int | Trädnodnivå. |

### postAlg(T el, int level) {#postAlg-T-int-}
```
public abstract void postAlg(T el, int level)
```


Kallas efter bearbetning av en nod i ett träd.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| el | T | Nod att bearbeta. |
| nivå | int | Trädnodnivå. |

### preAlg(T el, int level) {#preAlg-T-int-}
```
public abstract void preAlg(T el, int level)
```


Kallas före bearbetning av en nod i ett träd.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| el | T | Nod att bearbeta. |
| nivå | int | Trädnodnivå. |

