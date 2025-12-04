---
title: ICondition
second_title: Aspose.Tasks for Java API Reference
description: Represents a condition which can be used by filters or search methods.
type: docs
weight: 374
url: /java/com.aspose.tasks/icondition/
---
```
public interface ICondition<T>
```

Represents a condition which can be used by filters or search methods.

 T : The type of object to apply method interface to.
## Methods

| Method | Description |
| --- | --- |
| [check(T el)](#check-T-) | Returns true if the specified object satisfy the conditions. |
### check(T el) {#check-T-}
```
public abstract boolean check(T el)
```


Returns true if the specified object satisfy the conditions.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| el | T | The object to check. |

**Returns:**
boolean - True if the object satisfy the conditions.
