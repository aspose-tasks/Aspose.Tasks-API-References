---
title: "ITreeAlgorithm"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente un algorithme qui peut être appliqué à un arbre d'objets T."
type: docs
weight: 384
url: /fr/java/com.aspose.tasks/itreealgorithm/
---
```
public interface ITreeAlgorithm<T>
```

Représente un algorithme qui peut être appliqué à un arbre d'objets `T`.

T : Le type d'objet auquel appliquer l'interface de méthode.
## Méthodes

| Méthode | Description |
| --- | --- |
| [alg(T el, int level)](#alg-T-int-) | Traite un nœud d'un arbre. |
| [postAlg(T el, int level)](#postAlg-T-int-) | Appelé après le traitement d'un nœud d'un arbre. |
| [preAlg(T el, int level)](#preAlg-T-int-) | Appelé avant le traitement d'un nœud d'un arbre. |
### alg(T el, int level) {#alg-T-int-}
```
public abstract void alg(T el, int level)
```


Traite un nœud d'un arbre.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| el | T | Nœud à traiter. |
| niveau | int | Niveau du nœud d'arbre. |

### postAlg(T el, int level) {#postAlg-T-int-}
```
public abstract void postAlg(T el, int level)
```


Appelé après le traitement d'un nœud d'un arbre.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| el | T | Nœud à traiter. |
| niveau | int | Niveau du nœud d'arbre. |

### preAlg(T el, int level) {#preAlg-T-int-}
```
public abstract void preAlg(T el, int level)
```


Appelé avant le traitement d'un nœud d'un arbre.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| el | T | Nœud à traiter. |
| niveau | int | Niveau du nœud d'arbre. |

