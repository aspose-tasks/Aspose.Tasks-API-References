---
title: ITreeAlgorithm
second_title: Aspose.Tasks for Java API Reference
description: Represents an algorithm that can be applied to a tree of objects T.
type: docs
weight: 381
url: /java/com.aspose.tasks/itreealgorithm/
---
```
public interface ITreeAlgorithm<T>
```

Represents an algorithm that can be applied to a tree of objects `T`.

 T : The type of object to apply method interface to.
## Methods

| Method | Description |
| --- | --- |
| [alg(T el, int level)](#alg-T-int-) | Processes a node of a tree. |
| [postAlg(T el, int level)](#postAlg-T-int-) | Called after processing of a node of a tree. |
| [preAlg(T el, int level)](#preAlg-T-int-) | Called before processing of a node of a tree. |
### alg(T el, int level) {#alg-T-int-}
```
public abstract void alg(T el, int level)
```


Processes a node of a tree.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| el | T | Node to process. |
| level | int | Tree node level. |

### postAlg(T el, int level) {#postAlg-T-int-}
```
public abstract void postAlg(T el, int level)
```


Called after processing of a node of a tree.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| el | T | Node to process. |
| level | int | Tree node level. |

### preAlg(T el, int level) {#preAlg-T-int-}
```
public abstract void preAlg(T el, int level)
```


Called before processing of a node of a tree.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| el | T | Node to process. |
| level | int | Tree node level. |

