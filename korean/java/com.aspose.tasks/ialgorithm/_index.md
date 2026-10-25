---
title: "IAlgorithm"
second_title: "Aspose.Tasks for Java API Reference"
description: "T 객체 목록에 적용할 수 있는 알고리즘을 나타냅니다."
type: docs
weight: 375
url: /ko/java/com.aspose.tasks/ialgorithm/
---
```
public interface IAlgorithm<T>
```

`T` 객체 목록에 적용할 수 있는 알고리즘을 나타냅니다.

T : 메서드 인터페이스를 적용할 객체 유형.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [alg(T el, int index)](#alg-T-int-) | 목록의 객체를 처리합니다. |
| [postAlg(T el, int index)](#postAlg-T-int-) | 객체를 처리한 후에 호출됩니다. |
| [preAlg(T el, int index)](#preAlg-T-int-) | 객체를 처리하기 전에 호출됩니다. |
### alg(T el, int index) {#alg-T-int-}
```
public abstract void alg(T el, int index)
```


목록의 객체를 처리합니다. [preAlg(T, int)](../../com.aspose.tasks/ialgorithm\#preAlg-T--int-) 호출 후에;

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| el | T | 처리된 객체. |
| index | int | 객체의 인덱스. |

### postAlg(T el, int index) {#postAlg-T-int-}
```
public abstract void postAlg(T el, int index)
```


객체를 처리한 후에 호출됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| el | T | 처리된 객체. |
| index | int | 객체의 인덱스. |

### preAlg(T el, int index) {#preAlg-T-int-}
```
public abstract void preAlg(T el, int index)
```


객체를 처리하기 전에 호출됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| el | T | 처리된 객체. |
| index | int | 객체의 인덱스. |

