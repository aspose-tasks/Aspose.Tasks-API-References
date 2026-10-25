---
title: "非"
second_title: "Aspose.Tasks for Java API 参考"
description: "对指定条件应用逻辑非运算。"
type: docs
weight: 162
url: /zh/java/com.aspose.tasks/not/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class Not<T> implements ICondition<T>
```

对指定条件应用逻辑非运算。

T : 要将方法接口应用于的对象类型。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [Not(ICondition&lt;T&gt; condition)](#Not-com.aspose.tasks.ICondition-T--) | 初始化 Not&lt;T&gt; 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [check(T el)](#check-T-) | 如果指定的对象满足条件，则返回 true。 |
### Not(ICondition&lt;T&gt; condition) {#Not-com.aspose.tasks.ICondition-T--}
```
public Not(ICondition<T> condition)
```


初始化 Not&lt;T&gt; 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| condition | [ICondition](../../com.aspose.tasks/icondition) | 指定的条件。 |

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
