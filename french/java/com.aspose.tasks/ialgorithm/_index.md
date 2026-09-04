---
title: "IAlgorithm"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente un algorithme qui peut être appliqué à une liste d'objets T."
type: docs
weight: 375
url: /fr/java/com.aspose.tasks/ialgorithm/
---
```
public interface IAlgorithm<T>
```

Représente un algorithme qui peut être appliqué à une liste d'objets `T`.

T : Le type d'objet auquel appliquer l'interface de méthode.
## Méthodes

| Méthode | Description |
| --- | --- |
| [alg(T el, int index)](#alg-T-int-) | Traite un objet dans la liste. |
| [postAlg(T el, int index)](#postAlg-T-int-) | Appelé après le traitement d'un objet. |
| [preAlg(T el, int index)](#preAlg-T-int-) | Appelé avant le traitement d'un objet. |
### alg(T el, int index) {#alg-T-int-}
```
public abstract void alg(T el, int index)
```


Traite un objet dans la liste. Appelé après [preAlg(T, int)](../../com.aspose.tasks/ialgorithm\#preAlg-T--int-);

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| el | T | Objet traité. |
| indice | int | Index de l'objet. |

### postAlg(T el, int index) {#postAlg-T-int-}
```
public abstract void postAlg(T el, int index)
```


Appelé après le traitement d'un objet.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| el | T | Objet traité. |
| indice | int | Index de l'objet. |

### preAlg(T el, int index) {#preAlg-T-int-}
```
public abstract void preAlg(T el, int index)
```


Appelé avant le traitement d'un objet.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| el | T | Objet traité. |
| indice | int | Index de l'objet. |

