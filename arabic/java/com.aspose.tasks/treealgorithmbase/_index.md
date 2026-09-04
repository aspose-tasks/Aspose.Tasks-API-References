---
title: "TreeAlgorithmBase"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "فئة أساسية لتطبيقات ITreeAlgorithmltTgt"
type: docs
weight: 327
url: /ar/java/com.aspose.tasks/treealgorithmbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ITreeAlgorithm
```
public abstract class TreeAlgorithmBase<T> implements ITreeAlgorithm<T>
```

فئة أساسية لتطبيقات ITreeAlgorithm&lt;T&gt;

T : نوع العناصر.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [TreeAlgorithmBase()](#TreeAlgorithmBase--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [alg(T el, int level)](#alg-T-int-) | معالجة عقدة من شجرة. |
| [postAlg(T el, int level)](#postAlg-T-int-) | تم الاستدعاء بعد معالجة عقدة من شجرة. |
| [preAlg(T el, int level)](#preAlg-T-int-) | تم الاستدعاء قبل معالجة عقدة من شجرة. |
### TreeAlgorithmBase() {#TreeAlgorithmBase--}
```
public TreeAlgorithmBase()
```


### alg(T el, int level) {#alg-T-int-}
```
public abstract void alg(T el, int level)
```


معالجة عقدة من شجرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| el | T | العقدة للمعالجة. |
| المستوى | int | مستوى عقدة الشجرة. |

### postAlg(T el, int level) {#postAlg-T-int-}
```
public void postAlg(T el, int level)
```


تم الاستدعاء بعد معالجة عقدة من شجرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| el | T | العقدة للمعالجة. |
| المستوى | int | مستوى عقدة الشجرة. |

### preAlg(T el, int level) {#preAlg-T-int-}
```
public void preAlg(T el, int level)
```


تم الاستدعاء قبل معالجة عقدة من شجرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| el | T | العقدة للمعالجة. |
| المستوى | int | مستوى عقدة الشجرة. |

