---
title: "ListUtils"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "فئة مساعدة لمعالجة القوائم."
type: docs
weight: 147
url: /ar/java/com.aspose.tasks/listutils/
---

**Inheritance:**
java.lang.Object
```
public class ListUtils
```

فئة مساعدة لمعالجة القوائم.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [&lt;T&gt;apply(List&lt;T&gt; list, IAlgorithm&lt;T&gt; algorithm, int startIndex)](#-T-apply-java.util.List-T--com.aspose.tasks.IAlgorithm-T--int-) | تطبيق الخوارزمية على كل عنصر في القائمة بدءًا من الموضع المحدد. |
| [&lt;T&gt;filter(List&lt;T&gt; list, ICondition&lt;T&gt; cond)](#-T-filter-java.util.List-T--com.aspose.tasks.ICondition-T--) | تصفية عناصر القائمة وفقًا للشرط المحدد. |
| [&lt;T&gt;find(List&lt;T&gt; list, ICondition&lt;T&gt; cond, Class clazz)](#-T-find-java.util.List-T--com.aspose.tasks.ICondition-T--java.lang.Class-) | العثور على أول ظهور لعنصر في القائمة يحقق الشرط المحدد. |
### &lt;T&gt;apply(List&lt;T&gt; list, IAlgorithm&lt;T&gt; algorithm, int startIndex) {#-T-apply-java.util.List-T--com.aspose.tasks.IAlgorithm-T--int-}
```
public static void <T>apply(List<T> list, IAlgorithm<T> algorithm, int startIndex)
```


تطبيق الخوارزمية على كل عنصر في القائمة بدءًا من الموضع المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قائمة | java.util.List&lt;T&gt; | قائمة للمعالجة. |
| algorithm | [IAlgorithm](../../com.aspose.tasks/ialgorithm) | الخوارزمية المطبقة. |
| startIndex | int | موضع العنصر البداية. |

### &lt;T&gt;filter(List&lt;T&gt; list, ICondition&lt;T&gt; cond) {#-T-filter-java.util.List-T--com.aspose.tasks.ICondition-T--}
```
public static List<T> <T>filter(List<T> list, ICondition<T> cond)
```


تصفية عناصر القائمة وفقًا للشرط المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قائمة | java.util.List&lt;T&gt; | قائمة للمعالجة. |
| cond | [ICondition](../../com.aspose.tasks/icondition) | الشرط المستخدم لتصفية القائمة المحددة. |

**Returns:**
java.util.List&lt;T&gt; - قائمة مُفلترة.
### &lt;T&gt;find(List&lt;T&gt; list, ICondition&lt;T&gt; cond, Class clazz) {#-T-find-java.util.List-T--com.aspose.tasks.ICondition-T--java.lang.Class-}
```
public static T <T>find(List<T> list, ICondition<T> cond, Class clazz)
```


العثور على أول ظهور لعنصر في القائمة يحقق الشرط المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قائمة | java.util.List&lt;T&gt; | قائمة للمعالجة. |
| cond | [ICondition](../../com.aspose.tasks/icondition) | الشرط المستخدم للعثور على عنصر في القائمة المحددة. |
| clazz | java.lang.Class | نوع الفئة للعنصر T. |

**Returns:**
T - عنصر قائمة أو فارغ.
