---
title: "TreeAlgorithmBase"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Une classe de base pour les implémentations de ITreeAlgorithmltTgt"
type: docs
weight: 327
url: /fr/java/com.aspose.tasks/treealgorithmbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ITreeAlgorithm
```
public abstract class TreeAlgorithmBase<T> implements ITreeAlgorithm<T>
```

Une classe de base pour les implémentations de ITreeAlgorithm<T>

T : Le type des éléments.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [TreeAlgorithmBase()](#TreeAlgorithmBase--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [alg(T el, int level)](#alg-T-int-) | Traite un nœud d'un arbre. |
| [postAlg(T el, int level)](#postAlg-T-int-) | Appelé après le traitement d'un nœud d'un arbre. |
| [preAlg(T el, int level)](#preAlg-T-int-) | Appelé avant le traitement d'un nœud d'un arbre. |
### TreeAlgorithmBase() {#TreeAlgorithmBase--}
```
public TreeAlgorithmBase()
```


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
public void postAlg(T el, int level)
```


Appelé après le traitement d'un nœud d'un arbre.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| el | T | Nœud à traiter. |
| niveau | int | Niveau du nœud d'arbre. |

### preAlg(T el, int level) {#preAlg-T-int-}
```
public void preAlg(T el, int level)
```


Appelé avant le traitement d'un nœud d'un arbre.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| el | T | Nœud à traiter. |
| niveau | int | Niveau du nœud d'arbre. |

