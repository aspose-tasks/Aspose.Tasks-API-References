---
title: "TreeAlgorithmBase"
second_title: "Aspose.Tasks for Java API-referens"
description: "En basklass för implementationer av ITreeAlgorithmltTgt"
type: docs
weight: 327
url: /sv/java/com.aspose.tasks/treealgorithmbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ITreeAlgorithm
```
public abstract class TreeAlgorithmBase<T> implements ITreeAlgorithm<T>
```

En basklass för implementationer av ITreeAlgorithm&lt;T&gt;

T : Typen för elementen.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [TreeAlgorithmBase()](#TreeAlgorithmBase--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [alg(T el, int level)](#alg-T-int-) | Bearbetar en nod i ett träd. |
| [postAlg(T el, int level)](#postAlg-T-int-) | Kallas efter bearbetning av en nod i ett träd. |
| [preAlg(T el, int level)](#preAlg-T-int-) | Kallas före bearbetning av en nod i ett träd. |
### TreeAlgorithmBase() {#TreeAlgorithmBase--}
```
public TreeAlgorithmBase()
```


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
public void postAlg(T el, int level)
```


Kallas efter bearbetning av en nod i ett träd.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| el | T | Nod att bearbeta. |
| nivå | int | Trädnodnivå. |

### preAlg(T el, int level) {#preAlg-T-int-}
```
public void preAlg(T el, int level)
```


Kallas före bearbetning av en nod i ett träd.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| el | T | Nod att bearbeta. |
| nivå | int | Trädnodnivå. |

