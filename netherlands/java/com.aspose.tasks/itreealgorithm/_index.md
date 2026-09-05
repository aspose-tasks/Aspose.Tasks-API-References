---
title: "ITreeAlgorithm"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een algoritme voor dat kan worden toegepast op een boom van objecten T."
type: docs
weight: 384
url: /nl/java/com.aspose.tasks/itreealgorithm/
---
```
public interface ITreeAlgorithm<T>
```

Stelt een algoritme voor dat kan worden toegepast op een boom van objecten `T`.

T : Het type object waarop de methode‑interface moet worden toegepast.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [alg(T el, int level)](#alg-T-int-) | Verwerkt een knoop van een boom. |
| [postAlg(T el, int level)](#postAlg-T-int-) | Aangeroepen na het verwerken van een knoop van een boom. |
| [preAlg(T el, int level)](#preAlg-T-int-) | Aangeroepen vóór het verwerken van een knoop van een boom. |
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
public abstract void postAlg(T el, int level)
```


Aangeroepen na het verwerken van een knoop van een boom.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| el | T | Knooppunt om te verwerken. |
| niveau | int | Boomknooppuntniveau. |

### preAlg(T el, int level) {#preAlg-T-int-}
```
public abstract void preAlg(T el, int level)
```


Aangeroepen vóór het verwerken van een knoop van een boom.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| el | T | Knooppunt om te verwerken. |
| niveau | int | Boomknooppuntniveau. |

