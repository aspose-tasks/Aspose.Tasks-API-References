---
title: "و"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يطبق العملية المنطقية AND على الشروط المحددة."
type: docs
weight: 10
url: /ar/java/com.aspose.tasks/and/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class And<T> implements ICondition<T>
```

يطبق العملية المنطقية AND على الشروط المحددة.

T : نوع الكائن الذي سيتم تطبيق واجهة الطريقة عليه.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [And(ICondition&lt;T&gt; cond1, ICondition&lt;T&gt; cond2)](#And-com.aspose.tasks.ICondition-T--com.aspose.tasks.ICondition-T--) | يُنشئ مثيلاً جديداً لفئة And&lt;T&gt;. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [check(T el)](#check-T-) | يرجع true إذا كان الكائن المحدد يحقق الشروط. |
### And(ICondition&lt;T&gt; cond1, ICondition&lt;T&gt; cond2) {#And-com.aspose.tasks.ICondition-T--com.aspose.tasks.ICondition-T--}
```
public And(ICondition<T> cond1, ICondition<T> cond2)
```


يُنشئ مثيلاً جديداً لفئة And&lt;T&gt;.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cond1 | [ICondition](../../com.aspose.tasks/icondition) | الشرط الأول. |
| cond2 | [ICondition](../../com.aspose.tasks/icondition) | الشرط الثاني. |

### check(T el) {#check-T-}
```
public boolean check(T el)
```


يرجع true إذا كان الكائن المحدد يحقق الشروط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| el | T | الكائن المراد فحصه. |

**Returns:**
boolean - True إذا كان الكائن يحقق الشروط.
