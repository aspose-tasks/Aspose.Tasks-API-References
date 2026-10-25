---
title: "ITreeAlgorithm"
second_title: "Aspose.Tasks for Java API Reference"
description: "객체 T 트리에 적용할 수 있는 알고리즘을 나타냅니다."
type: docs
weight: 384
url: /ko/java/com.aspose.tasks/itreealgorithm/
---
```
public interface ITreeAlgorithm<T>
```

`T` 객체 트리에 적용될 수 있는 알고리즘을 나타냅니다.

T : 메서드 인터페이스를 적용할 객체 유형.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [alg(T el, int level)](#alg-T-int-) | 트리의 노드를 처리합니다. |
| [postAlg(T el, int level)](#postAlg-T-int-) | 트리 노드 처리 후에 호출됩니다. |
| [preAlg(T el, int level)](#preAlg-T-int-) | 트리 노드 처리 전에 호출됩니다. |
### alg(T el, int level) {#alg-T-int-}
```
public abstract void alg(T el, int level)
```


트리의 노드를 처리합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| el | T | 처리할 노드. |
| 레벨 | int | 트리 노드 레벨. |

### postAlg(T el, int level) {#postAlg-T-int-}
```
public abstract void postAlg(T el, int level)
```


트리 노드 처리 후에 호출됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| el | T | 처리할 노드. |
| 레벨 | int | 트리 노드 레벨. |

### preAlg(T el, int level) {#preAlg-T-int-}
```
public abstract void preAlg(T el, int level)
```


트리 노드 처리 전에 호출됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| el | T | 처리할 노드. |
| 레벨 | int | 트리 노드 레벨. |

