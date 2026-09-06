---
title: "ArrayUtils"
second_title: "Aspose.Tasks for Java API Referansı"
description: "ArrayList işleme için yardımcı sınıf."
type: docs
weight: 14
url: /tr/java/com.aspose.tasks/arrayutils/
---

**Inheritance:**
java.lang.Object
```
public class ArrayUtils
```

ArrayList işleme için yardımcı sınıf.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [&lt;T&gt;concat(Class&lt;T&gt; typeOfT, T[][] arrays)](#-T-concat-java.lang.Class-T--T--...-) |  |
| [apply(List array, IAlgorithm algorithm, int startIndex)](#apply-java.util.List-com.aspose.tasks.IAlgorithm-int-) | Belirtilen konumdan başlayarak her Liste öğesi için algoritmayı uygula. |
| [filter(List array, ICondition cond)](#filter-java.util.List-com.aspose.tasks.ICondition-) | ArrayList öğelerini belirtilen koşula göre filtrele. |
| [find(List array, ICondition cond)](#find-java.util.List-com.aspose.tasks.ICondition-) | Belirtilen koşulu sağlayan bir ArrayList öğesinin ilk oluşumunu bul. |
### &lt;T&gt;concat(Class&lt;T&gt; typeOfT, T[][] arrays) {#-T-concat-java.lang.Class-T--T--...-}
```
public static T[] <T>concat(Class<T> typeOfT, T[][] arrays)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| typeOfT | java.lang.Class&lt;T&gt; |  |
| diziler | T[][] |  |

**Returns:**
T[]
### apply(List array, IAlgorithm algorithm, int startIndex) {#apply-java.util.List-com.aspose.tasks.IAlgorithm-int-}
```
public static void apply(List array, IAlgorithm algorithm, int startIndex)
```


Belirtilen konumdan başlayarak her Liste öğesi için algoritmayı uygula.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizi | java.util.List | İşlenecek ArrayList. |
| algoritma | com.aspose.tasks.IAlgorithm | Uygulanan algoritma. |
| startIndex | int | Başlangıç öğesi konumu. |

### filter(List array, ICondition cond) {#filter-java.util.List-com.aspose.tasks.ICondition-}
```
public static List filter(List array, ICondition cond)
```


ArrayList öğelerini belirtilen koşula göre filtrele.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizi | java.util.List | İşlenecek liste. |
| cond | com.aspose.tasks.ICondition | Listeyi filtrelemek için kullanılan koşul. |

**Returns:**
java.util.List - Filtrelenmiş Liste.
### find(List array, ICondition cond) {#find-java.util.List-com.aspose.tasks.ICondition-}
```
public static Object find(List array, ICondition cond)
```


Belirtilen koşulu sağlayan bir ArrayList öğesinin ilk oluşumunu bul.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizi | java.util.List | İşlenecek ArrayList. |
| cond | com.aspose.tasks.ICondition | ArrayList öğesini bulmak için kullanılan koşul. |

**Returns:**
java.lang.Object - Liste öğesi veya null.
