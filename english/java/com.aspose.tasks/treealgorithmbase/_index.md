---
title: TreeAlgorithmBase
second_title: Aspose.Tasks for Java API Reference
description: A base class for implementations of ITreeAlgorithmltTgt
type: docs
weight: 324
url: /java/com.aspose.tasks/treealgorithmbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ITreeAlgorithm
```
public abstract class TreeAlgorithmBase<T> implements ITreeAlgorithm<T>
```

A base class for implementations of ITreeAlgorithm&lt;T&gt;

 T : The type of the elements.
## Constructors

| Constructor | Description |
| --- | --- |
| [TreeAlgorithmBase()](#TreeAlgorithmBase--) |  |
## Methods

| Method | Description |
| --- | --- |
| [alg(T el, int level)](#alg-T-int-) | Processes a node of a tree. |
| [postAlg(T el, int level)](#postAlg-T-int-) | Called after processing of a node of a tree. |
| [preAlg(T el, int level)](#preAlg-T-int-) | Called before processing of a node of a tree. |
### TreeAlgorithmBase() {#TreeAlgorithmBase--}
```
public TreeAlgorithmBase()
```


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
public void postAlg(T el, int level)
```


Called after processing of a node of a tree.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| el | T | Node to process. |
| level | int | Tree node level. |

### preAlg(T el, int level) {#preAlg-T-int-}
```
public void preAlg(T el, int level)
```


Called before processing of a node of a tree.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| el | T | Node to process. |
| level | int | Tree node level. |

