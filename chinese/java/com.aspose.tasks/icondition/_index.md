---
title: "ICondition"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示可被过滤器或搜索方法使用的条件。"
type: docs
weight: 377
url: /zh/java/com.aspose.tasks/icondition/
---
```
public interface ICondition<T>
```

表示可被过滤器或搜索方法使用的条件。

T : 要将方法接口应用于的对象类型。
## 方法

| 方法 | 描述 |
| --- | --- |
| [check(T el)](#check-T-) | 如果指定的对象满足条件，则返回 true。 |
### check(T el) {#check-T-}
```
public abstract boolean check(T el)
```


如果指定的对象满足条件，则返回 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| el | T | 要检查的对象。 |

**Returns:**
boolean - 如果对象满足条件，则为 True。
