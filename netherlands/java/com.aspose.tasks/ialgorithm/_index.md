---
title: "IAlgorithm"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een algoritme voor dat kan worden toegepast op een lijst van objecten T."
type: docs
weight: 375
url: /nl/java/com.aspose.tasks/ialgorithm/
---
```
public interface IAlgorithm<T>
```

Stelt een algoritme voor dat kan worden toegepast op een lijst van objecten `T`.

T : Het type object waarop de methode‑interface moet worden toegepast.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [alg(T el, int index)](#alg-T-int-) | Verwerkt een object in de lijst. |
| [postAlg(T el, int index)](#postAlg-T-int-) | Aangeroepen na het verwerken van een object. |
| [preAlg(T el, int index)](#preAlg-T-int-) | Aangeroepen vóór het verwerken van een object. |
### alg(T el, int index) {#alg-T-int-}
```
public abstract void alg(T el, int index)
```


Verwerkt een object in de lijst. Aangeroepen na [preAlg(T, int)](../../com.aspose.tasks/ialgorithm\#preAlg-T--int-);

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| el | T | Verwerkt object. |
| index | int | Index van het object. |

### postAlg(T el, int index) {#postAlg-T-int-}
```
public abstract void postAlg(T el, int index)
```


Aangeroepen na het verwerken van een object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| el | T | Verwerkt object. |
| index | int | Index van het object. |

### preAlg(T el, int index) {#preAlg-T-int-}
```
public abstract void preAlg(T el, int index)
```


Aangeroepen vóór het verwerken van een object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| el | T | Verwerkt object. |
| index | int | Index van het object. |

