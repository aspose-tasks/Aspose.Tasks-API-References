---
title: "ITreeAlgorithm"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل خوارزمية يمكن تطبيقها على شجرة من الكائنات T."
type: docs
weight: 384
url: /ar/java/com.aspose.tasks/itreealgorithm/
---
```
public interface ITreeAlgorithm<T>
```

يمثل خوارزمية يمكن تطبيقها على شجرة من الكائنات `T`.

T : نوع الكائن الذي سيتم تطبيق واجهة الطريقة عليه.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [alg(T el, int level)](#alg-T-int-) | معالجة عقدة من شجرة. |
| [postAlg(T el, int level)](#postAlg-T-int-) | تم الاستدعاء بعد معالجة عقدة من شجرة. |
| [preAlg(T el, int level)](#preAlg-T-int-) | تم الاستدعاء قبل معالجة عقدة من شجرة. |
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
public abstract void postAlg(T el, int level)
```


تم الاستدعاء بعد معالجة عقدة من شجرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| el | T | العقدة للمعالجة. |
| المستوى | int | مستوى عقدة الشجرة. |

### preAlg(T el, int level) {#preAlg-T-int-}
```
public abstract void preAlg(T el, int level)
```


تم الاستدعاء قبل معالجة عقدة من شجرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| el | T | العقدة للمعالجة. |
| المستوى | int | مستوى عقدة الشجرة. |

