---
title: "ArrayUtils"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Kelas utilitas untuk pemrosesan ArrayList."
type: docs
weight: 14
url: /id/java/com.aspose.tasks/arrayutils/
---

**Inheritance:**
java.lang.Object
```
public class ArrayUtils
```

Kelas utilitas untuk pemrosesan ArrayList.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [&lt;T&gt;concat(Class&lt;T&gt; typeOfT, T[][] arrays)](#-T-concat-java.lang.Class-T--T--...-) |  |
| [apply(List array, IAlgorithm algorithm, int startIndex)](#apply-java.util.List-com.aspose.tasks.IAlgorithm-int-) | Terapkan algoritma untuk setiap elemen List mulai dari posisi yang ditentukan. |
| [filter(List array, ICondition cond)](#filter-java.util.List-com.aspose.tasks.ICondition-) | Filter elemen ArrayList berdasarkan kondisi yang ditentukan. |
| [find(List array, ICondition cond)](#find-java.util.List-com.aspose.tasks.ICondition-) | Temukan kemunculan pertama dari elemen ArrayList yang memenuhi kondisi yang ditentukan. |
### &lt;T&gt;concat(Class&lt;T&gt; typeOfT, T[][] arrays) {#-T-concat-java.lang.Class-T--T--...-}
```
public static T[] <T>concat(Class<T> typeOfT, T[][] arrays)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| typeOfT | java.lang.Class&lt;T&gt; |  |
| array | T[][] |  |

**Returns:**
T[]
### apply(List array, IAlgorithm algorithm, int startIndex) {#apply-java.util.List-com.aspose.tasks.IAlgorithm-int-}
```
public static void apply(List array, IAlgorithm algorithm, int startIndex)
```


Terapkan algoritma untuk setiap elemen List mulai dari posisi yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| array | java.util.List | ArrayList untuk diproses. |
| algoritma | com.aspose.tasks.IAlgorithm | Algoritma yang diterapkan. |
| startIndex | int | Posisi elemen awal. |

### filter(List array, ICondition cond) {#filter-java.util.List-com.aspose.tasks.ICondition-}
```
public static List filter(List array, ICondition cond)
```


Filter elemen ArrayList berdasarkan kondisi yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| array | java.util.List | Daftar untuk diproses. |
| cond | com.aspose.tasks.ICondition | Kondisi yang digunakan untuk memfilter List. |

**Returns:**
java.util.List - List yang difilter.
### find(List array, ICondition cond) {#find-java.util.List-com.aspose.tasks.ICondition-}
```
public static Object find(List array, ICondition cond)
```


Temukan kemunculan pertama dari elemen ArrayList yang memenuhi kondisi yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| array | java.util.List | ArrayList untuk diproses. |
| cond | com.aspose.tasks.ICondition | Kondisi yang digunakan untuk menemukan elemen ArrayList. |

**Returns:**
java.lang.Object - Elemen List atau null.
