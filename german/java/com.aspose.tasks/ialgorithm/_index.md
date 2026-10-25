---
title: "IAlgorithm"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt einen Algorithmus dar, der auf eine Liste von Objekten T angewendet werden kann."
type: docs
weight: 375
url: /de/java/com.aspose.tasks/ialgorithm/
---
```
public interface IAlgorithm<T>
```

Stellt einen Algorithmus dar, der auf eine Liste von Objekten `T` angewendet werden kann.

T : Der Typ des Objekts, auf das die Methodenschnittstelle angewendet werden soll.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [alg(T el, int index)](#alg-T-int-) | Verarbeitet ein Objekt in der Liste. |
| [postAlg(T el, int index)](#postAlg-T-int-) | Wird nach der Verarbeitung eines Objekts aufgerufen. |
| [preAlg(T el, int index)](#preAlg-T-int-) | Wird vor der Verarbeitung eines Objekts aufgerufen. |
### alg(T el, int index) {#alg-T-int-}
```
public abstract void alg(T el, int index)
```


Verarbeitet ein Objekt in der Liste. Aufgerufen nach [preAlg(T, int)](../../com.aspose.tasks/ialgorithm\#preAlg-T--int-);

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| el | T | Verarbeitetes Objekt. |
| Index | int | Index des Objekts. |

### postAlg(T el, int index) {#postAlg-T-int-}
```
public abstract void postAlg(T el, int index)
```


Wird nach der Verarbeitung eines Objekts aufgerufen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| el | T | Verarbeitetes Objekt. |
| Index | int | Index des Objekts. |

### preAlg(T el, int index) {#preAlg-T-int-}
```
public abstract void preAlg(T el, int index)
```


Wird vor der Verarbeitung eines Objekts aufgerufen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| el | T | Verarbeitetes Objekt. |
| Index | int | Index des Objekts. |

