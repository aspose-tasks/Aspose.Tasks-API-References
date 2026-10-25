---
title: "TreeAlgorithmBase"
second_title: "Aspose.Tasks for Java API Reference"
description: "Eine Basisklasse für Implementierungen von ITreeAlgorithmltTgt"
type: docs
weight: 327
url: /de/java/com.aspose.tasks/treealgorithmbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ITreeAlgorithm
```
public abstract class TreeAlgorithmBase<T> implements ITreeAlgorithm<T>
```

Eine Basisklasse für Implementierungen von ITreeAlgorithm&lt;T&gt;

T : Der Typ der Elemente.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [TreeAlgorithmBase()](#TreeAlgorithmBase--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [alg(T el, int level)](#alg-T-int-) | Verarbeitet einen Knoten eines Baumes. |
| [postAlg(T el, int level)](#postAlg-T-int-) | Wird nach der Verarbeitung eines Knotens eines Baumes aufgerufen. |
| [preAlg(T el, int level)](#preAlg-T-int-) | Wird vor der Verarbeitung eines Knotens eines Baumes aufgerufen. |
### TreeAlgorithmBase() {#TreeAlgorithmBase--}
```
public TreeAlgorithmBase()
```


### alg(T el, int level) {#alg-T-int-}
```
public abstract void alg(T el, int level)
```


Verarbeitet einen Knoten eines Baumes.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| el | T | Zu verarbeitender Knoten. |
| Ebene | int | Baumknotenebene. |

### postAlg(T el, int level) {#postAlg-T-int-}
```
public void postAlg(T el, int level)
```


Wird nach der Verarbeitung eines Knotens eines Baumes aufgerufen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| el | T | Zu verarbeitender Knoten. |
| Ebene | int | Baumknotenebene. |

### preAlg(T el, int level) {#preAlg-T-int-}
```
public void preAlg(T el, int level)
```


Wird vor der Verarbeitung eines Knotens eines Baumes aufgerufen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| el | T | Zu verarbeitender Knoten. |
| Ebene | int | Baumknotenebene. |

