---
title: "ReadOnlyCollectionBase"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili koleksi objek hanya-baca."
type: docs
weight: 238
url: /id/java/com.aspose.tasks/readonlycollectionbase/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public abstract class ReadOnlyCollectionBase<T> extends AbstractList<T>
```

Mewakili koleksi objek hanya-baca.

T : Tipe item koleksi.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [add(T item)](#add-T-) | Ini adalah implementasi stub dari metode Add pada ICollection, yang hanya melempar UnsupportedOperationException |
| [add(int index, T element)](#add-int-T-) | \{@inheritDoc\} |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | Mengembalikan elemen pada indeks yang ditentukan. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Menentukan apakah koleksi hanya-baca. |
| [iterator()](#iterator--) | Mengembalikan enumerator untuk koleksi ini. |
| [remove(int index)](#remove-int-) | \{@inheritDoc\} |
| [remove(Object o)](#remove-java.lang.Object-) | \{@inheritDoc\} |
| [set(int index, T value)](#set-int-T-) | Mengembalikan elemen pada indeks yang ditentukan. |
| [size()](#size--) | Mendapatkan jumlah objek yang terkandung dalam objek. |
| [toList()](#toList--) | Mengonversi koleksi menjadi daftar objek. |
### add(T item) {#add-T-}
```
public final boolean add(T item)
```


Ini adalah implementasi stub dari metode Add pada ICollection, yang hanya melempar UnsupportedOperationException

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| item | T | Item yang akan ditambahkan. |

**Returns:**
boolean
### add(int index, T element) {#add-int-T-}
```
public final void add(int index, T element)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |
| elemen | T | \{@inheritDoc\} |

### clear() {#clear--}
```
public final void clear()
```




### contains(Object o) {#contains-java.lang.Object-}
```
public final boolean contains(Object o)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### get(int index) {#get-int-}
```
public final T get(int index)
```


Mengembalikan elemen pada indeks yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| index | int | Indeks berbasis nol dari elemen yang akan diambil. |

**Returns:**
T - elemen pada indeks yang ditentukan.
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public final int indexOf(Object o)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
int - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


Menentukan apakah koleksi hanya-baca.

**Returns:**
boolean - true jika koleksi hanya-baca; false sebaliknya.
### iterator() {#iterator--}
```
public final Iterator<T> iterator()
```


Mengembalikan enumerator untuk koleksi ini.

**Returns:**
java.util.Iterator<T> - Enumerator untuk koleksi ini.
### remove(int index) {#remove-int-}
```
public final T remove(int index)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
T - {@inheritDoc}
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### set(int index, T value) {#set-int-T-}
```
public final T set(int index, T value)
```


Mengembalikan elemen pada indeks yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| index | int | Indeks berbasis nol dari elemen yang akan diambil. |
| nilai | T |  |

**Returns:**
T - elemen pada indeks yang ditentukan.
### size() {#size--}
```
public final int size()
```


Mendapatkan jumlah objek yang terkandung dalam objek.

**Returns:**
int - jumlah objek yang terkandung dalam objek.
### toList() {#toList--}
```
public final List<T> toList()
```


Mengonversi koleksi menjadi daftar objek.

**Returns:**
java.util.List<T> - Daftar generik objek.
