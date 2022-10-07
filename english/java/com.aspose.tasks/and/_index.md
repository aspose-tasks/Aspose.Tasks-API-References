---
title: And
second_title: Aspose.Tasks for Java API Reference
description: Applies logical AND to the specified conditions.
type: docs
weight: 10
url: /java/com.aspose.tasks/and/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class And<T> implements ICondition<T>
```

Applies logical AND to the specified conditions.

 T : The type of object to apply method interface to.
## Constructors

| Constructor | Description |
| --- | --- |
| [And(ICondition&lt;T&gt; cond1, ICondition&lt;T&gt; cond2)](#And-com.aspose.tasks.ICondition-T--com.aspose.tasks.ICondition-T--) | Initializes a new instance of the  And\{T\}  class. |
## Methods

| Method | Description |
| --- | --- |
| [check(T el)](#check-T-) | Returns true if the specified object satisfy the conditions. |
### And(ICondition&lt;T&gt; cond1, ICondition&lt;T&gt; cond2) {#And-com.aspose.tasks.ICondition-T--com.aspose.tasks.ICondition-T--}
```
public And(ICondition<T> cond1, ICondition<T> cond2)
```


Initializes a new instance of the  And\{T\}  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cond1 | [ICondition](../../com.aspose.tasks/icondition) | First condition. |
| cond2 | [ICondition](../../com.aspose.tasks/icondition) | Second condition. |

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
