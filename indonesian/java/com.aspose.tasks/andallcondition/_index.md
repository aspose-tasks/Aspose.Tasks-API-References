---
title: "AndAllCondition"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Menerapkan AND logika pada semua kondisi."
type: docs
weight: 11
url: /id/java/com.aspose.tasks/andallcondition/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class AndAllCondition<T> implements ICondition<T>
```

Menerapkan logika AND pada semua kondisi. Misalnya: cond1 AND cond2 AND cond3...

T : Tipe objek untuk menerapkan antarmuka metode ke.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [AndAllCondition(List&lt;ICondition&lt;T&gt;&gt; conditions)](#AndAllCondition-java.util.List-com.aspose.tasks.ICondition-T---) | Menginisialisasi sebuah instance baru dari kelas AndAllCondition&lt;T&gt;. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [check(T el)](#check-T-) | Mengembalikan true jika objek yang ditentukan memenuhi kondisi. |
### AndAllCondition(List&lt;ICondition&lt;T&gt;&gt; conditions) {#AndAllCondition-java.util.List-com.aspose.tasks.ICondition-T---}
```
public AndAllCondition(List<ICondition<T>> conditions)
```


Menginisialisasi sebuah instance baru dari kelas AndAllCondition&lt;T&gt;.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| kondisi | java.util.List&lt;com.aspose.tasks.ICondition&lt;T&gt;&gt; | Daftar kondisi. |

### check(T el) {#check-T-}
```
public boolean check(T el)
```


Mengembalikan true jika objek yang ditentukan memenuhi kondisi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| el | T | Objek yang akan diperiksa. |

**Returns:**
boolean - True jika objek memenuhi kondisi.
