---
title: "TreeAlgorithmBase"
second_title: "Aspose.Tasks for Java API Reference"
description: "ITreeAlgorithmltTgt 구현을 위한 기본 클래스"
type: docs
weight: 327
url: /ko/java/com.aspose.tasks/treealgorithmbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ITreeAlgorithm
```
public abstract class TreeAlgorithmBase<T> implements ITreeAlgorithm<T>
```

ITreeAlgorithm&lt;T&gt; 구현을 위한 기본 클래스.

T : 요소의 유형.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [TreeAlgorithmBase()](#TreeAlgorithmBase--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [alg(T el, int level)](#alg-T-int-) | 트리의 노드를 처리합니다. |
| [postAlg(T el, int level)](#postAlg-T-int-) | 트리 노드 처리 후에 호출됩니다. |
| [preAlg(T el, int level)](#preAlg-T-int-) | 트리 노드 처리 전에 호출됩니다. |
### TreeAlgorithmBase() {#TreeAlgorithmBase--}
```
public TreeAlgorithmBase()
```


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
public void postAlg(T el, int level)
```


트리 노드 처리 후에 호출됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| el | T | 처리할 노드. |
| 레벨 | int | 트리 노드 레벨. |

### preAlg(T el, int level) {#preAlg-T-int-}
```
public void preAlg(T el, int level)
```


트리 노드 처리 전에 호출됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| el | T | 처리할 노드. |
| 레벨 | int | 트리 노드 레벨. |

