---
title: "AndAllCondition"
second_title: "Aspose.Tasks for Java API 参考"
description: "对所有条件应用逻辑 AND。"
type: docs
weight: 11
url: /zh/java/com.aspose.tasks/andallcondition/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class AndAllCondition<T> implements ICondition<T>
```

对所有条件应用逻辑 AND。例如：cond1 AND cond2 AND cond3...

T : 要将方法接口应用于的对象类型。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [AndAllCondition(List&lt;ICondition&lt;T&gt;&gt; conditions)](#AndAllCondition-java.util.List-com.aspose.tasks.ICondition-T---) | 初始化 AndAllCondition&lt;T&gt; 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [check(T el)](#check-T-) | 如果指定的对象满足条件，则返回 true。 |
### AndAllCondition(List&lt;ICondition&lt;T&gt;&gt; conditions) {#AndAllCondition-java.util.List-com.aspose.tasks.ICondition-T---}
```
public AndAllCondition(List<ICondition<T>> conditions)
```


初始化 AndAllCondition&lt;T&gt; 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 条件 | java.util.List&lt;com.aspose.tasks.ICondition&lt;T&gt;&gt; | 条件列表。 |

### check(T el) {#check-T-}
```
public boolean check(T el)
```


如果指定的对象满足条件，则返回 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| el | T | 要检查的对象。 |

**Returns:**
boolean - 如果对象满足条件，则为 True。
