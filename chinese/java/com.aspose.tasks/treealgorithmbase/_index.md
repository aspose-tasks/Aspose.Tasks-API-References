---
title: "TreeAlgorithmBase"
second_title: "Aspose.Tasks for Java API 参考"
description: "用于 ITreeAlgorithmltTgt 实现的基类。"
type: docs
weight: 327
url: /zh/java/com.aspose.tasks/treealgorithmbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ITreeAlgorithm
```
public abstract class TreeAlgorithmBase<T> implements ITreeAlgorithm<T>
```

ITreeAlgorithm<T> 实现的基类。

T：元素的类型。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [TreeAlgorithmBase()](#TreeAlgorithmBase--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [alg(T el, int level)](#alg-T-int-) | 处理树的一个节点。 |
| [postAlg(T el, int level)](#postAlg-T-int-) | 在处理树的节点之后调用。 |
| [preAlg(T el, int level)](#preAlg-T-int-) | 在处理树的节点之前调用。 |
### TreeAlgorithmBase() {#TreeAlgorithmBase--}
```
public TreeAlgorithmBase()
```


### alg(T el, int level) {#alg-T-int-}
```
public abstract void alg(T el, int level)
```


处理树的一个节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| el | T | 要处理的节点。 |
| 级别 | int | 树节点级别。 |

### postAlg(T el, int level) {#postAlg-T-int-}
```
public void postAlg(T el, int level)
```


在处理树的节点之后调用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| el | T | 要处理的节点。 |
| 级别 | int | 树节点级别。 |

### preAlg(T el, int level) {#preAlg-T-int-}
```
public void preAlg(T el, int level)
```


在处理树的节点之前调用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| el | T | 要处理的节点。 |
| 级别 | int | 树节点级别。 |

