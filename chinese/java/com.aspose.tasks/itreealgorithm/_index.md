---
title: "ITreeAlgorithm"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示可应用于对象树 T 的算法。"
type: docs
weight: 384
url: /zh/java/com.aspose.tasks/itreealgorithm/
---
```
public interface ITreeAlgorithm<T>
```

表示一种可应用于对象树 `T` 的算法。

T : 要将方法接口应用于的对象类型。
## 方法

| 方法 | 描述 |
| --- | --- |
| [alg(T el, int level)](#alg-T-int-) | 处理树的一个节点。 |
| [postAlg(T el, int level)](#postAlg-T-int-) | 在处理树的节点之后调用。 |
| [preAlg(T el, int level)](#preAlg-T-int-) | 在处理树的节点之前调用。 |
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
public abstract void postAlg(T el, int level)
```


在处理树的节点之后调用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| el | T | 要处理的节点。 |
| 级别 | int | 树节点级别。 |

### preAlg(T el, int level) {#preAlg-T-int-}
```
public abstract void preAlg(T el, int level)
```


在处理树的节点之前调用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| el | T | 要处理的节点。 |
| 级别 | int | 树节点级别。 |

