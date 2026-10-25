---
title: "ListUtils"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Liste işleme için yardımcı sınıf."
type: docs
weight: 147
url: /tr/java/com.aspose.tasks/listutils/
---

**Inheritance:**
java.lang.Object
```
public class ListUtils
```

Liste işleme için yardımcı sınıf.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [&lt;T&gt;apply(List&lt;T&gt; list, IAlgorithm&lt;T&gt; algorithm, int startIndex)](#-T-apply-java.util.List-T--com.aspose.tasks.IAlgorithm-T--int-) | Belirtilen konumdan başlayarak listedeki her öğeye algoritma uygula. |
| [&lt;T&gt;filter(List&lt;T&gt; list, ICondition&lt;T&gt; cond)](#-T-filter-java.util.List-T--com.aspose.tasks.ICondition-T--) | Liste öğelerini belirtilen koşula göre filtrele. |
| [&lt;T&gt;find(List&lt;T&gt; list, ICondition&lt;T&gt; cond, Class clazz)](#-T-find-java.util.List-T--com.aspose.tasks.ICondition-T--java.lang.Class-) | Belirtilen koşulu sağlayan bir liste öğesinin ilk oluşumunu bul. |
### &lt;T&gt;apply(List&lt;T&gt; list, IAlgorithm&lt;T&gt; algorithm, int startIndex) {#-T-apply-java.util.List-T--com.aspose.tasks.IAlgorithm-T--int-}
```
public static void <T>apply(List<T> list, IAlgorithm<T> algorithm, int startIndex)
```


Belirtilen konumdan başlayarak listedeki her öğeye algoritma uygula.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| liste | java.util.List&lt;T&gt; | İşlenecek liste. |
| algorithm | [IAlgorithm](../../com.aspose.tasks/ialgorithm) | Uygulanan algoritma. |
| startIndex | int | Başlangıç öğesi konumu. |

### &lt;T&gt;filter(List&lt;T&gt; list, ICondition&lt;T&gt; cond) {#-T-filter-java.util.List-T--com.aspose.tasks.ICondition-T--}
```
public static List<T> <T>filter(List<T> list, ICondition<T> cond)
```


Liste öğelerini belirtilen koşula göre filtrele.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| liste | java.util.List&lt;T&gt; | İşlenecek bir liste. |
| cond | [ICondition](../../com.aspose.tasks/icondition) | Belirtilen listeyi filtrelemek için kullanılan koşul. |

**Returns:**
java.util.List&lt;T&gt; - Filtrelenmiş liste.
### &lt;T&gt;find(List&lt;T&gt; list, ICondition&lt;T&gt; cond, Class clazz) {#-T-find-java.util.List-T--com.aspose.tasks.ICondition-T--java.lang.Class-}
```
public static T <T>find(List<T> list, ICondition<T> cond, Class clazz)
```


Belirtilen koşulu sağlayan bir liste öğesinin ilk oluşumunu bul.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| liste | java.util.List&lt;T&gt; | İşlenecek bir liste. |
| cond | [ICondition](../../com.aspose.tasks/icondition) | Belirtilen listede bir öğe bulmak için kullanılan koşul. |
| clazz | java.lang.Class | T öğesinin sınıf tipi. |

**Returns:**
T - Liste öğesi veya null.
