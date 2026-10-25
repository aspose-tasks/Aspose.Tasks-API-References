---
title: "IAlgorithm"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示一种可以应用于对象 T 列表的算法。"
type: docs
weight: 375
url: /zh/java/com.aspose.tasks/ialgorithm/
---
```
public interface IAlgorithm<T>
```

表示可应用于对象列表 `T` 的算法。

T : 要将方法接口应用于的对象类型。
## 方法

| 方法 | 描述 |
| --- | --- |
| [alg(T el, int index)](#alg-T-int-) | 处理列表中的对象。 |
| [postAlg(T el, int index)](#postAlg-T-int-) | 在对象处理后调用。 |
| [preAlg(T el, int index)](#preAlg-T-int-) | 在对象处理前调用。 |
### alg(T el, int index) {#alg-T-int-}
```
public abstract void alg(T el, int index)
```


处理列表中的对象。 在 [preAlg(T, int)](../../com.aspose.tasks/ialgorithm\#preAlg-T--int-) 之后调用；

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| el | T | 已处理的对象。 |
| 索引 | int | 对象的索引。 |

### postAlg(T el, int index) {#postAlg-T-int-}
```
public abstract void postAlg(T el, int index)
```


在对象处理后调用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| el | T | 已处理的对象。 |
| 索引 | int | 对象的索引。 |

### preAlg(T el, int index) {#preAlg-T-int-}
```
public abstract void preAlg(T el, int index)
```


在对象处理前调用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| el | T | 已处理的对象。 |
| 索引 | int | 对象的索引。 |

