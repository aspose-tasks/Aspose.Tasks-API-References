---
title: "IAlgorithm"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل خوارزمية يمكن تطبيقها على قائمة من الكائنات T."
type: docs
weight: 375
url: /ar/java/com.aspose.tasks/ialgorithm/
---
```
public interface IAlgorithm<T>
```

يمثل خوارزمية يمكن تطبيقها على قائمة من الكائنات `T`.

T : نوع الكائن الذي سيتم تطبيق واجهة الطريقة عليه.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [alg(T el, int index)](#alg-T-int-) | يعالج كائنًا في القائمة. |
| [postAlg(T el, int index)](#postAlg-T-int-) | يُستدعى بعد معالجة كائن. |
| [preAlg(T el, int index)](#preAlg-T-int-) | يُستدعى قبل معالجة كائن. |
### alg(T el, int index) {#alg-T-int-}
```
public abstract void alg(T el, int index)
```


يعالج كائنًا في القائمة. يتم استدعاؤه بعد [preAlg(T, int)](../../com.aspose.tasks/ialgorithm\#preAlg-T--int-);

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| el | T | الكائن المعالج. |
| فهرس | int | فهرس الكائن. |

### postAlg(T el, int index) {#postAlg-T-int-}
```
public abstract void postAlg(T el, int index)
```


يُستدعى بعد معالجة كائن.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| el | T | الكائن المعالج. |
| فهرس | int | فهرس الكائن. |

### preAlg(T el, int index) {#preAlg-T-int-}
```
public abstract void preAlg(T el, int index)
```


يُستدعى قبل معالجة كائن.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| el | T | الكائن المعالج. |
| فهرس | int | فهرس الكائن. |

