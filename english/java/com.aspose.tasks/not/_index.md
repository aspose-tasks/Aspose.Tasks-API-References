---
title: Not
second_title: Aspose.Tasks for Java API Reference
description: Applies logical NOT to the specified condition.
type: docs
weight: 152
url: /java/com.aspose.tasks/not/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class Not<T> implements ICondition<T>
```

Applies logical NOT to the specified condition.

 T : The type of object to apply method interface to.
## Constructors

| Constructor | Description |
| --- | --- |
| [Not(ICondition&lt;T&gt; condition)](#Not-com.aspose.tasks.ICondition-T--) | Initializes a new instance of the Not&lt;T&gt; class. |
## Methods

| Method | Description |
| --- | --- |
| [check(T el)](#check-T-) | Returns true if the specified object satisfy the condition. |
### Not(ICondition&lt;T&gt; condition) {#Not-com.aspose.tasks.ICondition-T--}
```
public Not(ICondition<T> condition)
```


Initializes a new instance of the Not&lt;T&gt; class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| condition | [ICondition](../../com.aspose.tasks/icondition) | Specified condition. |

### check(T el) {#check-T-}
```
public boolean check(T el)
```


Returns true if the specified object satisfy the condition.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| el | T | The object to check. |

**Returns:**
boolean - True if the object satisfy the condition.
