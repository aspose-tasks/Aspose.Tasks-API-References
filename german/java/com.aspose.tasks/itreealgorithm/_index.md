---
title: "ITreeAlgorithm"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt einen Algorithmus dar, der auf einen Baum von Objekten T angewendet werden kann."
type: docs
weight: 384
url: /de/java/com.aspose.tasks/itreealgorithm/
---
```
public interface ITreeAlgorithm<T>
```

Stellt einen Algorithmus dar, der auf einen Objektbaum `T` angewendet werden kann.

T : Der Typ des Objekts, auf das die Methodenschnittstelle angewendet werden soll.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [alg(T el, int level)](#alg-T-int-) | Verarbeitet einen Knoten eines Baumes. |
| [postAlg(T el, int level)](#postAlg-T-int-) | Wird nach der Verarbeitung eines Knotens eines Baumes aufgerufen. |
| [preAlg(T el, int level)](#preAlg-T-int-) | Wird vor der Verarbeitung eines Knotens eines Baumes aufgerufen. |
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
public abstract void postAlg(T el, int level)
```


Wird nach der Verarbeitung eines Knotens eines Baumes aufgerufen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| el | T | Zu verarbeitender Knoten. |
| Ebene | int | Baumknotenebene. |

### preAlg(T el, int level) {#preAlg-T-int-}
```
public abstract void preAlg(T el, int level)
```


Wird vor der Verarbeitung eines Knotens eines Baumes aufgerufen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| el | T | Zu verarbeitender Knoten. |
| Ebene | int | Baumknotenebene. |

