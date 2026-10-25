---
title: "Not"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Menerapkan NOT logika pada kondisi yang ditentukan."
type: docs
weight: 162
url: /id/java/com.aspose.tasks/not/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class Not<T> implements ICondition<T>
```

Menerapkan NOT logika pada kondisi yang ditentukan.

T : Tipe objek untuk menerapkan antarmuka metode ke.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [Not(ICondition&lt;T&gt; condition)](#Not-com.aspose.tasks.ICondition-T--) | Menginisialisasi instance baru dari kelas Not&lt;T&gt;. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [check(T el)](#check-T-) | Mengembalikan true jika objek yang ditentukan memenuhi kondisi. |
### Not(ICondition&lt;T&gt; condition) {#Not-com.aspose.tasks.ICondition-T--}
```
public Not(ICondition<T> condition)
```


Menginisialisasi instance baru dari kelas Not&lt;T&gt;.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| condition | [ICondition](../../com.aspose.tasks/icondition) | Kondisi yang ditentukan. |

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
