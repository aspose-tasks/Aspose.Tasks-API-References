---
title: IAlgorithm
second_title: Aspose.Tasks for Java API Reference
description: Represents an algorithm that can be applied to a list of objects T.
type: docs
weight: 374
url: /java/com.aspose.tasks/ialgorithm/
---
```
public interface IAlgorithm<T>
```

Represents an algorithm that can be applied to a list of objects `T`.

 T : The type of object to apply method interface to.
## Methods

| Method | Description |
| --- | --- |
| [alg(T el, int index)](#alg-T-int-) | Processes an object in the list. |
| [postAlg(T el, int index)](#postAlg-T-int-) | Called after processing of an object. |
| [preAlg(T el, int index)](#preAlg-T-int-) | Called before processing of an object. |
### alg(T el, int index) {#alg-T-int-}
```
public abstract void alg(T el, int index)
```


Processes an object in the list. Called after [preAlg(T, int)](../../com.aspose.tasks/ialgorithm\#preAlg-T--int-);

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| el | T | Processed object. |
| index | int | Index of the object. |

### postAlg(T el, int index) {#postAlg-T-int-}
```
public abstract void postAlg(T el, int index)
```


Called after processing of an object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| el | T | Processed object. |
| index | int | Index of the object. |

### preAlg(T el, int index) {#preAlg-T-int-}
```
public abstract void preAlg(T el, int index)
```


Called before processing of an object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| el | T | Processed object. |
| index | int | Index of the object. |

