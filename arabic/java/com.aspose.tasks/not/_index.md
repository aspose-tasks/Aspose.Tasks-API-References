---
title: "ليس"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يطبق NOT المنطقي على الشرط المحدد."
type: docs
weight: 162
url: /ar/java/com.aspose.tasks/not/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class Not<T> implements ICondition<T>
```

يطبق NOT المنطقي على الشرط المحدد.

T : نوع الكائن الذي سيتم تطبيق واجهة الطريقة عليه.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [Not(ICondition&lt;T&gt; condition)](#Not-com.aspose.tasks.ICondition-T--) | يُنشئ مثيلاً جديداً من الفئة Not&lt;T&gt;. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [check(T el)](#check-T-) | يرجع true إذا كان الكائن المحدد يحقق الشرط. |
### Not(ICondition&lt;T&gt; condition) {#Not-com.aspose.tasks.ICondition-T--}
```
public Not(ICondition<T> condition)
```


يُنشئ مثيلاً جديداً من الفئة Not&lt;T&gt;.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| condition | [ICondition](../../com.aspose.tasks/icondition) | الشرط المحدد. |

### check(T el) {#check-T-}
```
public boolean check(T el)
```


يرجع true إذا كان الكائن المحدد يحقق الشرط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| el | T | الكائن المراد فحصه. |

**Returns:**
boolean - True إذا كان الكائن يحقق الشرط.
