---
title: "ArrayUtils"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "فئة مساعدة لمعالجة ArrayList."
type: docs
weight: 14
url: /ar/java/com.aspose.tasks/arrayutils/
---

**Inheritance:**
java.lang.Object
```
public class ArrayUtils
```

فئة مساعدة لمعالجة ArrayList.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [&lt;T&gt;concat(Class&lt;T&gt; typeOfT, T[][] arrays)](#-T-concat-java.lang.Class-T--T--...-) |  |
| [apply(List array, IAlgorithm algorithm, int startIndex)](#apply-java.util.List-com.aspose.tasks.IAlgorithm-int-) | تطبيق الخوارزمية على كل عنصر في القائمة بدءًا من الموضع المحدد. |
| [filter(List array, ICondition cond)](#filter-java.util.List-com.aspose.tasks.ICondition-) | تصفية عناصر ArrayList وفقًا للشرط المحدد. |
| [find(List array, ICondition cond)](#find-java.util.List-com.aspose.tasks.ICondition-) | العثور على أول ظهور لعنصر ArrayList يحقق الشرط المحدد. |
### &lt;T&gt;concat(Class&lt;T&gt; typeOfT, T[][] arrays) {#-T-concat-java.lang.Class-T--T--...-}
```
public static T[] <T>concat(Class<T> typeOfT, T[][] arrays)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| typeOfT | java.lang.Class&lt;T&gt; |  |
| المصفوفات | T[][] |  |

**Returns:**
T[]
### apply(List array, IAlgorithm algorithm, int startIndex) {#apply-java.util.List-com.aspose.tasks.IAlgorithm-int-}
```
public static void apply(List array, IAlgorithm algorithm, int startIndex)
```


تطبيق الخوارزمية على كل عنصر في القائمة بدءًا من الموضع المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| مصفوفة | java.util.List | ArrayList للمعالجة. |
| الخوارزمية | com.aspose.tasks.IAlgorithm | الخوارزمية المطبقة. |
| startIndex | int | موضع العنصر البداية. |

### filter(List array, ICondition cond) {#filter-java.util.List-com.aspose.tasks.ICondition-}
```
public static List filter(List array, ICondition cond)
```


تصفية عناصر ArrayList وفقًا للشرط المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| مصفوفة | java.util.List | قائمة للمعالجة. |
| cond | com.aspose.tasks.ICondition | الشرط المستخدم لتصفية القائمة. |

**Returns:**
java.util.List - القائمة المصفاة.
### find(List array, ICondition cond) {#find-java.util.List-com.aspose.tasks.ICondition-}
```
public static Object find(List array, ICondition cond)
```


العثور على أول ظهور لعنصر ArrayList يحقق الشرط المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| مصفوفة | java.util.List | ArrayList للمعالجة. |
| cond | com.aspose.tasks.ICondition | الشرط المستخدم للعثور على عنصر ArrayList. |

**Returns:**
java.lang.Object - عنصر قائمة أو فارغ.
