---
title: "TreeAlgorithmBase"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Een basisklasse voor implementaties van ITreeAlgorithmltTgt"
type: docs
weight: 327
url: /nl/java/com.aspose.tasks/treealgorithmbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ITreeAlgorithm
```
public abstract class TreeAlgorithmBase<T> implements ITreeAlgorithm<T>
```

Een basisklasse voor implementaties van ITreeAlgorithm&lt;T&gt;

T : Het type van de elementen.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [TreeAlgorithmBase()](#TreeAlgorithmBase--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [alg(T el, int level)](#alg-T-int-) | Verwerkt een knoop van een boom. |
| [postAlg(T el, int level)](#postAlg-T-int-) | Aangeroepen na het verwerken van een knoop van een boom. |
| [preAlg(T el, int level)](#preAlg-T-int-) | Aangeroepen vóór het verwerken van een knoop van een boom. |
### TreeAlgorithmBase() {#TreeAlgorithmBase--}
```
public TreeAlgorithmBase()
```


### alg(T el, int level) {#alg-T-int-}
```
public abstract void alg(T el, int level)
```


Verwerkt een knoop van een boom.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| el | T | Knooppunt om te verwerken. |
| niveau | int | Boomknooppuntniveau. |

### postAlg(T el, int level) {#postAlg-T-int-}
```
public void postAlg(T el, int level)
```


Aangeroepen na het verwerken van een knoop van een boom.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| el | T | Knooppunt om te verwerken. |
| niveau | int | Boomknooppuntniveau. |

### preAlg(T el, int level) {#preAlg-T-int-}
```
public void preAlg(T el, int level)
```


Aangeroepen vóór het verwerken van een knoop van een boom.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| el | T | Knooppunt om te verwerken. |
| niveau | int | Boomknooppuntniveau. |

