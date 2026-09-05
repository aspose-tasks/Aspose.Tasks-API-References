---
title: "ListUtils"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Kelas utilitas untuk pemrosesan daftar."
type: docs
weight: 147
url: /id/java/com.aspose.tasks/listutils/
---

**Inheritance:**
java.lang.Object
```
public class ListUtils
```

Kelas utilitas untuk pemrosesan daftar.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [&lt;T&gt;apply(List&lt;T&gt; list, IAlgorithm&lt;T&gt; algorithm, int startIndex)](#-T-apply-java.util.List-T--com.aspose.tasks.IAlgorithm-T--int-) | Terapkan algoritma untuk setiap elemen daftar mulai dari posisi yang ditentukan. |
| [&lt;T&gt;filter(List&lt;T&gt; list, ICondition&lt;T&gt; cond)](#-T-filter-java.util.List-T--com.aspose.tasks.ICondition-T--) | Filter elemen daftar berdasarkan kondisi yang ditentukan. |
| [&lt;T&gt;find(List&lt;T&gt; list, ICondition&lt;T&gt; cond, Class clazz)](#-T-find-java.util.List-T--com.aspose.tasks.ICondition-T--java.lang.Class-) | Temukan kemunculan pertama elemen daftar yang memenuhi kondisi yang ditentukan. |
### &lt;T&gt;apply(List&lt;T&gt; list, IAlgorithm&lt;T&gt; algorithm, int startIndex) {#-T-apply-java.util.List-T--com.aspose.tasks.IAlgorithm-T--int-}
```
public static void <T>apply(List<T> list, IAlgorithm<T> algorithm, int startIndex)
```


Terapkan algoritma untuk setiap elemen daftar mulai dari posisi yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| daftar | java.util.List&lt;T&gt; | Daftar untuk diproses. |
| algorithm | [IAlgorithm](../../com.aspose.tasks/ialgorithm) | Algoritma yang diterapkan. |
| startIndex | int | Posisi elemen awal. |

### &lt;T&gt;filter(List&lt;T&gt; list, ICondition&lt;T&gt; cond) {#-T-filter-java.util.List-T--com.aspose.tasks.ICondition-T--}
```
public static List<T> <T>filter(List<T> list, ICondition<T> cond)
```


Filter elemen daftar berdasarkan kondisi yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| daftar | java.util.List&lt;T&gt; | Sebuah daftar untuk diproses. |
| cond | [ICondition](../../com.aspose.tasks/icondition) | Kondisi yang digunakan untuk memfilter daftar yang ditentukan. |

**Returns:**
java.util.List&lt;T&gt; - Daftar yang difilter.
### &lt;T&gt;find(List&lt;T&gt; list, ICondition&lt;T&gt; cond, Class clazz) {#-T-find-java.util.List-T--com.aspose.tasks.ICondition-T--java.lang.Class-}
```
public static T <T>find(List<T> list, ICondition<T> cond, Class clazz)
```


Temukan kemunculan pertama elemen daftar yang memenuhi kondisi yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| daftar | java.util.List&lt;T&gt; | Sebuah daftar untuk diproses. |
| cond | [ICondition](../../com.aspose.tasks/icondition) | Kondisi yang digunakan untuk menemukan elemen dalam daftar yang ditentukan. |
| clazz | java.lang.Class | Tipe kelas dari elemen T. |

**Returns:**
T - Elemen daftar atau null.
