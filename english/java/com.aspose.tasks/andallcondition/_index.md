---
title: AndAllCondition
second_title: Aspose.Tasks for Java API Reference
description: Applies logical AND to all conditions.
type: docs
weight: 11
url: /java/com.aspose.tasks/andallcondition/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class AndAllCondition<T> implements ICondition<T>
```

Applies logical AND to all conditions. For example: cond1 AND cond2 AND cond3...

 T : The type of object to apply method interface to.
## Constructors

| Constructor | Description |
| --- | --- |
| [AndAllCondition(List&lt;ICondition&lt;T&gt;&gt; conditions)](#AndAllCondition-java.util.List-com.aspose.tasks.ICondition-T---) | Initializes a new instance of the  AndAllCondition\{T\}  class. |
## Methods

| Method | Description |
| --- | --- |
| [check(T el)](#check-T-) | Returns true if the specified object satisfy the conditions. |
### AndAllCondition(List&lt;ICondition&lt;T&gt;&gt; conditions) {#AndAllCondition-java.util.List-com.aspose.tasks.ICondition-T---}
```
public AndAllCondition(List<ICondition<T>> conditions)
```


Initializes a new instance of the  AndAllCondition\{T\}  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| conditions | java.util.List&lt;com.aspose.tasks.ICondition&lt;T&gt;&gt; | The list of conditions. |

### check(T el) {#check-T-}
```
public boolean check(T el)
```


Returns true if the specified object satisfy the conditions.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| el | T | The object to check. |

**Returns:**
boolean - True if the object satisfy the conditions.
