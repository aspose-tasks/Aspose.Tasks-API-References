---
title: "与"
second_title: "Aspose.Tasks for Java API 参考"
description: "对指定条件应用逻辑 AND。"
type: docs
weight: 10
url: /zh/java/com.aspose.tasks/and/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class And<T> implements ICondition<T>
```

对指定条件应用逻辑 AND。

T : 要将方法接口应用于的对象类型。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [And(ICondition&lt;T&gt; cond1, ICondition&lt;T&gt; cond2)](#And-com.aspose.tasks.ICondition-T--com.aspose.tasks.ICondition-T--) | 初始化 And&lt;T&gt; 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [check(T el)](#check-T-) | 如果指定的对象满足条件，则返回 true。 |
### And(ICondition&lt;T&gt; cond1, ICondition&lt;T&gt; cond2) {#And-com.aspose.tasks.ICondition-T--com.aspose.tasks.ICondition-T--}
```
public And(ICondition<T> cond1, ICondition<T> cond2)
```


初始化 And&lt;T&gt; 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cond1 | [ICondition](../../com.aspose.tasks/icondition) | 第一条件。 |
| cond2 | [ICondition](../../com.aspose.tasks/icondition) | 第二条件。 |

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
