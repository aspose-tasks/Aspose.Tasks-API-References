---
title: "Dan"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Menerapkan AND logika pada kondisi yang ditentukan."
type: docs
weight: 10
url: /id/java/com.aspose.tasks/and/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class And<T> implements ICondition<T>
```

Menerapkan AND logika pada kondisi yang ditentukan.

T : Tipe objek untuk menerapkan antarmuka metode ke.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [And(ICondition&lt;T&gt; cond1, ICondition&lt;T&gt; cond2)](#And-com.aspose.tasks.ICondition-T--com.aspose.tasks.ICondition-T--) | Menginisialisasi instance baru dari kelas And&lt;T&gt;. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [check(T el)](#check-T-) | Mengembalikan true jika objek yang ditentukan memenuhi kondisi. |
### And(ICondition&lt;T&gt; cond1, ICondition&lt;T&gt; cond2) {#And-com.aspose.tasks.ICondition-T--com.aspose.tasks.ICondition-T--}
```
public And(ICondition<T> cond1, ICondition<T> cond2)
```


Menginisialisasi instance baru dari kelas And&lt;T&gt;.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| cond1 | [ICondition](../../com.aspose.tasks/icondition) | Kondisi pertama. |
| cond2 | [ICondition](../../com.aspose.tasks/icondition) | Kondisi kedua. |

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
