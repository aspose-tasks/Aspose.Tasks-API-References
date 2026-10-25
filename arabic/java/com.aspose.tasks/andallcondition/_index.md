---
title: "AndAllCondition"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يطبق العملية المنطقية AND على جميع الشروط."
type: docs
weight: 11
url: /ar/java/com.aspose.tasks/andallcondition/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class AndAllCondition<T> implements ICondition<T>
```

يطبق العملية المنطقية AND على جميع الشروط. على سبيل المثال: cond1 AND cond2 AND cond3...

T : نوع الكائن الذي سيتم تطبيق واجهة الطريقة عليه.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [AndAllCondition(List&lt;ICondition&lt;T&gt;&gt; conditions)](#AndAllCondition-java.util.List-com.aspose.tasks.ICondition-T---) | ينشئ مثلاً جديداً من الفئة AndAllCondition&lt;T&gt;. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [check(T el)](#check-T-) | يرجع true إذا كان الكائن المحدد يحقق الشروط. |
### AndAllCondition(List&lt;ICondition&lt;T&gt;&gt; conditions) {#AndAllCondition-java.util.List-com.aspose.tasks.ICondition-T---}
```
public AndAllCondition(List<ICondition<T>> conditions)
```


ينشئ مثلاً جديداً من الفئة AndAllCondition&lt;T&gt;.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الشروط | java.util.List&lt;com.aspose.tasks.ICondition&lt;T&gt;&gt; | قائمة الشروط. |

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
